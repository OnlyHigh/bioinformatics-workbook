Many times the results generated by the bioinformatics programs are either simple text files (tab/comma seperated), pdf files or in some rare cases png/jpeg files. Here we will show you how to view these files without having to download them locally to your machine.  

### Text files ###

The text files are the easiest. You can use any of the standard UNIX commands to view them. There are many commands for this purpose such as:

<tr><td><table class="tableizer-table"></td></tr>
<tr><td><thead><tr class="tableizer-firstrow"><th>Command</th><th>Purpose</th><th>Example</th><th>Use cases</th></tr></thead><tbody></td></tr>
 <tr><td> <tr><td><blockcode>less</blockcode></td><td>view file pagewise with more options</td><td><blockcode>less</blockcode> <i>filename</i></td><td>use <blockcode>-S</blockcode> to avoid line wrapping, you can use arrow keys to scroll</td></tr></td></tr>
 <tr><td> <tr><td><blockcode>more</blockcode></td><td>view file pagewise</td><td><blockcode>more</blockcode> <i>filename</i></td><td>use <blockcode>less</blockcode> instead</td></tr></td></tr>
 <tr><td> <tr><td><blockcode>cat</blockcode></td><td>catalogs the contents of a file</td><td><blockcode>cat</blockcode> <i>filename</i></td><td>you can send the contenst of a file to clipboard or to another file using this command</td></tr></td></tr>
 <tr><td> <tr><td><blockcode>tac</blockcode></td><td>reverse of cat, reverses the order of lines</td><td><blockcode>tac</blockcode> <i>filename</i></td><td>pipe this to <blockcode>less</blockcode> commad to scroll through the file in reverse</td></tr></td></tr>
 <tr><td> <tr><td><blockcode>head</blockcode></td><td>view first few lines of a file</td><td><blockcode>head</blockcode> <i>filename</i></td><td>use <blockcode>-n</blockcode> option to change the number of lines displayed. <blockcode>-n 20</blockcode> displays 20 lines</td></tr></td></tr>
 <tr><td> <tr><td><blockcode>tail</blockcode></td><td>view last few lines of a file</td><td><blockcode>tail</blockcode> <i>filename</i></td><td>use <blockcode> -n</blockcode> option to change the number of lines displayed. <blockcode>-n 20</blockcode> displays 20 lines</td></tr></td></tr>
 <tr><td> <tr><td><blockcode>od</blockcode></td><td>octal dump of a file </td><td><blockcode>od</blockcode> <i>filename</i></td><td>use<blockcode> -c</blockcode> options and pipe it through less. You can see non printable characters with this option (like tab, whitespace, newline etc)</td></tr></td></tr>
 <tr><td></tbody></table></td></tr>
</tbody></table>


### PDF files ###

Most HPC's allows X11 forwarding. You can enable this when you are logging in to the remote host using the `-X` option. For eg.,
<pre>
ssh -X arnstrm@condodtn.its.iastate.edu
</pre>
Once logged in, you can now open any GUI interface programs on the remote-host and it appears as a new window in your local machine. Although, there are plenty of program options to open a `pdf` file, you can almost always find the `firefox` browser in every machine. This should be sufficient to open a `PDF` file. To get started, type:
<pre>
firefox
</pre>

A new window will open, then go to `file` >> `open file` >> _select the pdf file you want to open_ .
If you don't find the menu tab, pressing `alt` + `f` should bring up the `file` menu


### PNG files ###

Again, you need X11 forwarding enabled to do this. If your machine has `imagemagick` module installed, load it:

<pre>
module load imagemagick
</pre>
To open any picture files, you can just do:
<pre>
display filename.png
</pre>

If you don't have this program installed, you can try the `firefox` method. Although, to view `png` files, you may have to install the addon before you open the file. Addons are easy to add, once the firefox is opened, press `ctrl` + `shift` + `A`, that will open `add-ons` page (you can also just type `about:addons` to open this). Search for [_Perfect View_](https://addons.mozilla.org/en-us/firefox/addon/perfect-view/) add-on, and add it to your `firefox`. Now you can open the file normally as you opened the `pdf` files.
