---
Title: actionGetMailLayoutTransformations
hidden: true
hookTitle: 'Define the transformation to apply on layout'
files:
    -
        url: 'https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/MailTemplate/MailTemplateTwigRenderer.php'
        file: src/Adapter/MailTemplate/MailTemplateTwigRenderer.php
locations:
    - 'front office'
type: action
hookAliases: 
hasExample: true
array_return: false
check_exceptions: false
chain: false
origin: core
description: 'This hook allows to add/remove TransformationInterface used to generate an email layout'

---

{{% hookDescriptor %}}

## Call of the Hook in the origin file

```php
dispatchWithParameters(
            MailTemplateRendererInterface::GET_MAIL_LAYOUT_TRANSFORMATIONS,
            [
                'mailLayout' => $mailLayout,
                'templateType' => $templateType,
                'layoutTransformations' => $templateTransformations,
            ]
        )
```

## Example implementation

This hook has been implemented as an example in our [modules examples repository - example_module_mailtheme](https://github.com/PrestaShop/example-modules/blob/8.x/example_module_mailtheme).
