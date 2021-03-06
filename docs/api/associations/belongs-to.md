<a name="belongsto"></a>
# Mixin BelongsTo
[View code](https://github.com/sequelize/sequelize/blob/95f8fc2783814cd61ec1a8d623b23cd6a7cd5e17/lib/associations/belongs-to.js#L17)
One-to-one association

In the API reference below, replace `Assocation` with the actual name of your association, e.g. for `User.belongsTo(Project)` the getter will be `user.getProject()`.


***

<a name="getassociation"></a>
## `getAssociation([options])` -> `Promise.<Instance>`
[View code](https://github.com/sequelize/sequelize/blob/95f8fc2783814cd61ec1a8d623b23cd6a7cd5e17/lib/associations/belongs-to.js#L82)
Get the associated instance


**Params:**

| Name | Type | Description |
| ---- | ---- | ----------- |
| [options] | Object |  |
| [options.scope] | String &#124; Boolean | Apply a scope on the related model, or remove its default scope by passing false. |


***

<a name="setassociation"></a>
## `setAssociation([newAssociation], [options])` -> `Promise`
[View code](https://github.com/sequelize/sequelize/blob/95f8fc2783814cd61ec1a8d623b23cd6a7cd5e17/lib/associations/belongs-to.js#L92)
Set the associated model


**Params:**

| Name | Type | Description |
| ---- | ---- | ----------- |
| [newAssociation] | Instance &#124; String &#124; Number | An instance or the primary key of an instance to associate with this. Pass `null` or `undefined` to remove the association. |
| [options] | Object | Options passed to `this.save` |
| [options.save=true] | Boolean | Skip saving this after setting the foreign key if false. |


***

<a name="createassociation"></a>
## `createAssociation([values], [options])` -> `Promise`
[View code](https://github.com/sequelize/sequelize/blob/95f8fc2783814cd61ec1a8d623b23cd6a7cd5e17/lib/associations/belongs-to.js#L101)
Create a new instance of the associated model and associate it with this.


**Params:**

| Name | Type | Description |
| ---- | ---- | ----------- |
| [values] | Object |  |
| [options] | Object | Options passed to `target.create` and setAssociation. |


***

_This document is automatically generated based on source code comments. Please do not edit it directly, as your changes will be ignored. Please write on <a href="irc://irc.freenode.net/#sequelizejs">IRC</a>, open an issue or a create a pull request if you feel something can be improved. For help on how to write source code documentation see [JSDoc](http://usejsdoc.org) and [dox](https://github.com/tj/dox)_