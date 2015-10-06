# InkExport
A Bash script that exports selected objects from a svg to multiple resolution icons for android.

It will generate images of the following resolutions:

| Resolution | Dimension |
|---------|:-------------|
|	Default | 48 x 48 px   |
| ldpi    | 36 x 36 px   |
| mdpi    | 48 x 48 px   |
| hdpi    | 72 x 72 px   |
| xhdpi   | 96 x 96 px   |
| xxhdpi  | 144 x 144 px |
| xxxhdpi | 192 x 192 px | 

Installation
---

`git clone https://github.com/JeyKeu/InkExport.git && cd InkExport && chmod +x inkexport && sudo cp inkexport /usr/local/bin/inkexport`

Usage
---
To display help orusage instructions type:
`inkexport` or `inkexport -h`
To Export icons from Inkscape:

`inkexport -f <Path-To-Svg>#<Object-Id> (REQUIRED)`

"Example:"

`inkexport -f my_vector.svg#Id-Of-Object-To-Export`

Switches
---
`InkExport` accepts the following switches:

| Switch          | Description |
|-----------------|:-------------|
|	-h or no switch | When excuted with `-h` or without any switch at all, it will display the usage     |
| -f              | This switch is required. -f takes a file as argument. This is the input svg file   |
| -s              | Do not show generated files    |


Workfolw
---

- Create your icon in `Inkscape` 
- Resize it to be large
- Set a sensible ID to the object or group from the `Object Properties` dialog
- Save the file as svg
- Open Terminal
- Enter `inkexport -f your.svg#myIcon`
- Generated files are displayed in your default file browser

License
---

MIT

