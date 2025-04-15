---
Title: action<FormName>FormBuilderModifier
hidden: true
hookTitle: 
files:
    -
        url: 'https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Core/Form/IdentifiableObject/Builder/FormBuilder.php'
        file: src/Core/Form/IdentifiableObject/Builder/FormBuilder.php
locations:
    - 'front office'
    - 'back office'
type: action
hookAliases: 
hasExample: true
array_return: false
check_exceptions: false
chain: false
origin: core
description: "This hook allows to modify an identifiable object forms content by modifying form builder data or FormBuilder itself.\nReplace FormBuilderName by the identitiable object type."

---

{{% hookDescriptor %}}

## Call of the Hook in the origin file

```php
$this->hookDispatcher->dispatchWithParameters('action' . $this->camelize($formBuilder->getName()) . 'FormBuilderModifier', [
    'form_builder' => $formBuilder,
    'data' => &$data,
    'options' => &$options,
    'id' => $id
]);
```

## Example implementation

This hook has been implemented as an example in our [modules examples repository - demoextendsymfonyform1](https://github.com/PrestaShop/example-modules/tree/8.x/demoextendsymfonyform1).

This hook has been implemented as an example in our [modules examples repository - demoextendsymfonyform2](https://github.com/PrestaShop/example-modules/tree/8.x/demoextendsymfonyform2).

This hook has been implemented as an example in our [modules examples repository - demoextendsymfonyform3](https://github.com/PrestaShop/example-modules/tree/8.x/demoextendsymfonyform3).

This hook has been implemented as an example in our [modules examples repository - demoproductform](https://github.com/PrestaShop/example-modules/tree/8.x/demoproductform).

This hook has been described in the context of Product Page in Back Office in [Extending the new product page form page]({{< relref "/8/modules/sample-modules/extend-product-page" >}})
