### CSS rahlo obarva vsako drugo vrstico.

![](https://github.com/SRP-B/Scripts/assets/152384379/6327b1a7-18f8-47a5-a4cd-cb64c6024cf8)


#### Edge 
- https://microsoftedge.microsoft.com/addons/detail/custom-style-script/eocdolakkgkbmnfojgicnicdnmimfhoo
- Za `podpora.sigov.si` dodaj CSS:
```
table.plinner > tbody > tr:nth-child(4n+3):has(a.rsd) {
    background-color: lightgray;
  }

```

# Firefox
-	odpreš `about:config` nastaviš `toolkit.legacyUserProfileCustomizations.stylesheets` > true
-	odpreš `about:profiles` open root directory in premakneš `userContent.css` v `chrome/userContent.css`
