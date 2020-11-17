### *Quick navigation*

[Home](./index.md) | [Tag manager Basics](./tag-manager-basics.md) | [Form templates](./form-templates.md) | [Form creation](./form-creation.md) | [Form display](./form-display.md) | [Form reporting](./form-reporting.md) | [About](./about.md)

# Form display | Matomo feedback forms
When you created your first form you can publish the form to the site where you are running Matomo.

Forms are injected through Matomos Tag Manager (as tags).

When you go to the TagManager interface, you can create a new type of tags called "User Feedback".
You will be able to select the wich form to display in the tag and you will also be able to customize how the form will be displayed.

## Display options

You can display the form as an overlay or as a oure html form.

You can also adjust where to inject the form in the page (default is en of the body). This gives you the ability to place a form as part of your existing content.

Styling
We try to only apply styling that makes the form Accecible and responsive by default.
However: A form will always inherit your sites CSS so the end result will always be based in your sites css.

We offer a field called custom CSS on the tag, where you could add custom styles. But a better option is probably to add the styles properly into your sites style sheets.

### Display rules
You can control how often the form should be displayed to a user throug the default tag options in Matomo.

You could also possibly set up any kind of advanced rules through the TagManager (this is really a huge benefit of using the tagmanager in Matomo for display of tags)


 