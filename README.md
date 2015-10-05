# InkExport
A Bash script that exports selected objects from a svg to multiple resolution icons for android.
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

Workfolw
---

- Create your icon in `Inkscape` 
- Resize it to be large
- Set sensible ID to the object or group from the `Object Properties` dialog
- Save the file as svg
- Open Terminal
- Enter `inkexport -f your.svg#myIcon`

License
---

MIT

