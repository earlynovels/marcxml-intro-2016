# END Training XML Resources


![national union catalog](https://github.com/earlynovels/training/blob/master/img/nuc1.jpg)

---

These are a few links that point to resources regarding MARC files and editing XML more generally. Do feel free to email me if you have any questions!

[nkashya1@swarthmore.edu](mailto:nkashya1@swarthmore.edu)

## LINKS

### Reference

- [Wonderfully dated MARC overview through Libraries Linking Idaho](http://lili.org/forlibs/ce/able/course8/04marchistory.htm)
- [MARC reference guide](http://www.loc.gov/marc/bibliographic/)
- [OpenRefine Tutorials & Docs](https://github.com/OpenRefine/OpenRefine/wiki)
- [Owen Stephens' posts on converting between MarcEdit and OpenRefine](http://www.meanboyfriend.com/overdue_ideas/2015/07/worked-example-fixing-marc-data-1/)_included for completeness, no expectations that you be able to follow this tutorial unless interested_

### Software

- [OpenRefine](http://openrefine.org/) 
- [MarcEdit](http://marcedit.reeset.net/downloads)
- [Online XML Validator](http://xmlvalidation.com/)
- **_For Macs:_** [TextWrangler](http://www.barebones.com/products/textwrangler/)
- **_For PCs:_** [Notepad++](https://notepad-plus-plus.org/download/v6.9.2.html)

### Tidying up XML in the text editor

#### TextWrangler

(not many steps but potentially a little scary)

``` 
#!/bin/sh
XMLLINT_INDENT=$'\t' xmllint --format --encode utf-8 -
```

1. open a new file in TextWrangler
2. cut & paste the code snippet above
3. save to file named `TidyXML.sh`
4. move this file to the following folder: `~/Library/Application Support/TextWrangler/Text Filters/`
**_Note:_** If the `Library` folder does not appear under `/Users/[username]/` in Finder, simply hold down the `option` key
5. restart TextWrangler, now under `Text > Text Filters` you should see an option for `TidyXML`

#### Notepad++

1. open plugin manager: `Plugins > Plugin Manager`
2. select XML Tools from the install menu: `Install > XML Tools`
3. under `Plugins > XML Tools` you should now see an option for Pretty Print which should automatically format your XML file

