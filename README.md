Twitter Bootstrap Theme for Symfony2's Form Framework
-----------------------------------------------------

This is a simple, not entirely complete implementation of Twitter's Bootstrap for use in Symfony2's form framework. 

For my usage, I've installed this layout file into a Core bundle under the path like `CoreBundle/Resources/views/Form/bootstrap_layout.html.twig`

Using the theme in a single form
================================

Add the following to one of your view files:

```
{% form_theme yourForm 'Core:Form:bootstrap_layout.html.twig' %}
```

Using the theme across your entire application
==============================================

Add the following to your `config.yml`

```yml
# Twig Configuration
twig:
    form:
        resources:
            - 'Core:Form:bootstrap_layout.html.twig'
````