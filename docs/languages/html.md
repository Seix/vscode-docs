---
Order: 6
Area: languages
TOCTitle: HTML
ContentId: 43095EAF-4B93-407C-A6F9-6DB173D79088
PageTitle: HTML Programming with Visual Studio Code
DateApproved: 9/8/2016
MetaDescription: Get the best out of Visual Studio Code for HTML development
---

# HTML Programming in VS Code

VS Code provides basic support for HTML programming out of the box. Install an extension for greater functionality. 

<div class="marketplace-extensions-html"></div>

> Tip: The extensions shown above are dynamically queried. Click on an extension tile above to read the description and reviews to decide which extension is best for you. See more in the [Marketplace](https://marketplace.visualstudio.com).

## IntelliSense

As you type in HTML, we offer suggestions via HTML IntelliSense.  In the image below you can see a suggested HTML element closure `</div>` as well as a context specific list of suggested elements.

![HTML IntelliSense](images/html/htmlintellisense.png)

We also offer up suggestions for elements, tags, some values (as defined in HTML 5), Ionic and AngularJS tags. You can trigger suggestions at any time by pressing `kb(editor.action.triggerSuggest)`.

You can also control which built-in code completion providers are active. Override these in your user or workspace [settings](/docs/customization/userandworkspace.md) if you prefer not to see the corresponding suggestions.

```json
// Configures if the built-in HTML language suggests Angular V1 tags and properties.
"html.suggest.angular1": true,

// Configures if the built-in HTML language suggests Ionic tags, properties and values.
"html.suggest.ionic": true,

// Configures if the built-in HTML language suggests HTML5 tags, properties and values.
"html.suggest.html5": true
```

## Format HTML

To improve the formatting of your HTML code press `kb(editor.action.format)` and the selected area will be reformatted.

>**Tip:** Configure the HTML formatter settings in the [User and Workspace Settings](/docs/customization/userandworkspace.md).

## Emmet snippets

We support Emmet snippet expansion, simply press `kb(editor.emmet.action.expandAbbreviation)`.

![Emmet HTML support built-in](images/html/emmetsnippet.gif)

>**Tip:** See the HTML section of the [Emmet cheat sheet](http://docs.emmet.io/cheat-sheet) for valid abbreviations.

If you'd like to use HTML Emmet abbreviations with other languages, you can associate an Emmet syntax profile (such as `html`, `css`) with other languages with the `emmet.syntaxProfiles` [setting](/docs/customization/userandworkspace.md). The setting takes a [language id](/docs/languages/overview.md#language-id) and associates it with an Emmet profile.

For example, to use Emmet HTML abbreviations inside JavaScript:

```json
{
    "emmet.syntaxProfiles": {
        "javascript": "html"
     }
}
```

We also support [User Defined Snippets](/docs/customization/userdefinedsnippets.md).

## Next Steps

Read on to find out about:

* [CSS, Less and Sass](/docs/languages/css.md) - VS Code has first class support for CSS including Less and Sass.


