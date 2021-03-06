# Alert

---

## Alert Skins

{{#docs-demo as |demo|}}
  {{#demo.example name='au-alert-skins.hbs'}}
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit"  @alertskin={{"info"}}>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
    </AuAlert>
    <AuAlert @alertIcon="check" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"success"}}>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
    </AuAlert>
    <AuAlert @alertIcon="alert-triangle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"warning"}}>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
    </AuAlert>
    <AuAlert @alertIcon="cross" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"error"}}>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
    </AuAlert>
  {{/demo.example}}
  {{demo.snippet 'au-alert-skins.hbs'}}
{{/docs-demo}}

## Alert Action

{{#docs-demo as |demo|}}
  {{#demo.example name='au-alert-action.hbs'}}
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}}>
      <p class="au-u-margin-bottom">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
      <AuButton>Primary action</AuButton>
      <AuButton @skin="secondary">Secondary action</AuButton>
    </AuAlert>
  {{/demo.example}}
  {{demo.snippet 'au-alert-action.hbs'}}
{{/docs-demo}}

## Alert Smaller Sizes

{{#docs-demo as |demo|}}
  {{#demo.example name='au-alert-sizes.hbs'}}
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @alertsize={{"small"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @alertsize={{"tiny"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>

  {{/demo.example}}
  {{demo.snippet 'au-alert-sizes.hbs'}}
{{/docs-demo}}


## Alert Closable

{{#docs-demo as |demo|}}
  {{#demo.example name='au-alert-closable.hbs'}}
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @closable={{true}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @alertsize={{"small"}} @closable={{true}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @alertsize={{"tiny"}} @closable={{true}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>

  {{/demo.example}}
  {{demo.snippet 'au-alert-closable.hbs'}}
{{/docs-demo}}


## Alert Content Variations

{{#docs-demo as |demo|}}
  {{#demo.example name='au-alert-content.hbs'}}
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @alertsize={{"small"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertIcon="info-circle" @alertTitle="Sunt in culpa qui officia deserunt mollit" @alertskin={{"info"}} @alertsize={{"tiny"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>

    <AuAlert @alertIcon="info-circle" @alertskin={{"info"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertIcon="info-circle" @alertskin={{"info"}} @alertsize={{"small"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
    <AuAlert @alertskin={{"info"}} @alertsize={{"tiny"}}>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
    </AuAlert>
  {{/demo.example}}
  {{demo.snippet 'au-alert-content.hbs'}}
{{/docs-demo}}

## Arguments

| Argument      | Description | Type | Default value |
| ------------- | ----------- | ---- | ------------- |
| `@alertSkin` | Sets the style of the alert  | `value`: `info` / `success` / `warning` / `error` | - |
| `@alertIcon` | Add an icon to the alert | `value`: <AuLink @linkRoute="docs.atoms.au-icon">Find the options here</AuLink> | - |
| `@alertSize` | Set the size of the alert | `value`: `small` / `default` | `default` |
| `@alertTitle` | Add a title to the alert | `String` | - |
| `@closable` | Makes the alert closable | `Boolean` | `false` |
