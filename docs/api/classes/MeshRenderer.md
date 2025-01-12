# Class: MeshRenderer

The mesh renderer component is a component used to render the mesh

## Hierarchy

- `RenderNode`

  ↳ **`MeshRenderer`**

  ↳↳ [`GUIRenderer`](GUIRenderer.md)

  ↳↳ [`SkinnedMeshRenderer`](SkinnedMeshRenderer.md)

  ↳↳ [`SkyRenderer`](SkyRenderer.md)

### Constructors

- [constructor](MeshRenderer.md#constructor)

### Properties

- [object3D](MeshRenderer.md#object3d)
- [isDestroyed](MeshRenderer.md#isdestroyed)
- [receiveShadow](MeshRenderer.md#receiveshadow)
- [instanceCount](MeshRenderer.md#instancecount)
- [lodLevel](MeshRenderer.md#lodlevel)
- [alwaysRender](MeshRenderer.md#alwaysrender)
- [instanceID](MeshRenderer.md#instanceid)
- [drawType](MeshRenderer.md#drawtype)
- [isRenderOrderChange](MeshRenderer.md#isrenderorderchange)
- [needSortOnCameraZ](MeshRenderer.md#needsortoncameraz)
- [preInit](MeshRenderer.md#preinit)

### Accessors

- [eventDispatcher](MeshRenderer.md#eventdispatcher)
- [isStart](MeshRenderer.md#isstart)
- [transform](MeshRenderer.md#transform)
- [enable](MeshRenderer.md#enable)
- [geometry](MeshRenderer.md#geometry)
- [material](MeshRenderer.md#material)
- [renderOrder](MeshRenderer.md#renderorder)
- [rendererMask](MeshRenderer.md#renderermask)
- [materials](MeshRenderer.md#materials)
- [castShadow](MeshRenderer.md#castshadow)
- [castGI](MeshRenderer.md#castgi)
- [castReflection](MeshRenderer.md#castreflection)

### Methods

- [start](MeshRenderer.md#start)
- [stop](MeshRenderer.md#stop)
- [onUpdate](MeshRenderer.md#onupdate)
- [onLateUpdate](MeshRenderer.md#onlateupdate)
- [onBeforeUpdate](MeshRenderer.md#onbeforeupdate)
- [onGraphic](MeshRenderer.md#ongraphic)
- [onParentChange](MeshRenderer.md#onparentchange)
- [onEnable](MeshRenderer.md#onenable)
- [onDisable](MeshRenderer.md#ondisable)
- [cloneTo](MeshRenderer.md#cloneto)
- [copyComponent](MeshRenderer.md#copycomponent)
- [setMorphInfluence](MeshRenderer.md#setmorphinfluence)
- [setMorphInfluenceIndex](MeshRenderer.md#setmorphinfluenceindex)
- [onCompute](MeshRenderer.md#oncompute)
- [destroy](MeshRenderer.md#destroy)
- [init](MeshRenderer.md#init)
- [attachSceneOctree](MeshRenderer.md#attachsceneoctree)
- [detachSceneOctree](MeshRenderer.md#detachsceneoctree)
- [addMask](MeshRenderer.md#addmask)
- [removeMask](MeshRenderer.md#removemask)
- [hasMask](MeshRenderer.md#hasmask)
- [addRendererMask](MeshRenderer.md#addrenderermask)
- [removeRendererMask](MeshRenderer.md#removerenderermask)
- [selfCloneMaterials](MeshRenderer.md#selfclonematerials)
- [renderPass](MeshRenderer.md#renderpass)
- [renderPass2](MeshRenderer.md#renderpass2)
- [recordRenderPass2](MeshRenderer.md#recordrenderpass2)
- [beforeDestroy](MeshRenderer.md#beforedestroy)

## Constructors

### constructor

• **new MeshRenderer**()

#### Overrides

RenderNode.constructor

#### Defined in

[src/components/renderer/MeshRenderer.ts:24](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L24)

## Properties

### object3D

• **object3D**: [`Object3D`](Object3D.md) = `null`

owner object3D

#### Inherited from

RenderNode.object3D

#### Defined in

[src/components/ComponentBase.ts:17](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L17)

___

### isDestroyed

• `Optional` **isDestroyed**: `boolean`

#### Inherited from

RenderNode.isDestroyed

#### Defined in

[src/components/ComponentBase.ts:38](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L38)

___

### receiveShadow

• **receiveShadow**: `boolean`

Enabling this option allows the grid to display any shadows cast on the grid.

#### Defined in

[src/components/renderer/MeshRenderer.ts:21](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L21)

___

### instanceCount

• **instanceCount**: `number` = `0`

#### Inherited from

RenderNode.instanceCount

#### Defined in

[src/components/renderer/RenderNode.ts:33](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L33)

___

### lodLevel

• **lodLevel**: `number` = `0`

#### Inherited from

RenderNode.lodLevel

#### Defined in

[src/components/renderer/RenderNode.ts:34](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L34)

___

### alwaysRender

• **alwaysRender**: `boolean` = `false`

#### Inherited from

RenderNode.alwaysRender

#### Defined in

[src/components/renderer/RenderNode.ts:35](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L35)

___

### instanceID

• **instanceID**: `string`

#### Inherited from

RenderNode.instanceID

#### Defined in

[src/components/renderer/RenderNode.ts:36](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L36)

___

### drawType

• **drawType**: `number` = `0`

#### Inherited from

RenderNode.drawType

#### Defined in

[src/components/renderer/RenderNode.ts:37](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L37)

___

### isRenderOrderChange

• `Optional` **isRenderOrderChange**: `boolean`

#### Inherited from

RenderNode.isRenderOrderChange

#### Defined in

[src/components/renderer/RenderNode.ts:52](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L52)

___

### needSortOnCameraZ

• `Optional` **needSortOnCameraZ**: `boolean`

#### Inherited from

RenderNode.needSortOnCameraZ

#### Defined in

[src/components/renderer/RenderNode.ts:53](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L53)

___

### preInit

• **preInit**: `boolean` = `false`

#### Inherited from

RenderNode.preInit

#### Defined in

[src/components/renderer/RenderNode.ts:56](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L56)

## Accessors

### eventDispatcher

• `get` **eventDispatcher**(): [`CEventDispatcher`](CEventDispatcher.md)

#### Returns

[`CEventDispatcher`](CEventDispatcher.md)

#### Inherited from

RenderNode.eventDispatcher

#### Defined in

[src/components/ComponentBase.ts:23](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L23)

• `set` **eventDispatcher**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`CEventDispatcher`](CEventDispatcher.md) |

#### Returns

`void`

#### Inherited from

RenderNode.eventDispatcher

#### Defined in

[src/components/ComponentBase.ts:28](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L28)

___

### isStart

• `get` **isStart**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderNode.isStart

#### Defined in

[src/components/ComponentBase.ts:40](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L40)

___

### transform

• `get` **transform**(): [`Transform`](Transform.md)

Return the Transform component attached to the Object3D.

#### Returns

[`Transform`](Transform.md)

#### Inherited from

RenderNode.transform

#### Defined in

[src/components/ComponentBase.ts:47](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L47)

___

### enable

• `get` **enable**(): `boolean`

Enable/disable components. The enabled components can be updated, while the disabled components cannot be updated.

#### Returns

`boolean`

#### Inherited from

RenderNode.enable

#### Defined in

[src/components/ComponentBase.ts:68](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L68)

• `set` **enable**(`value`): `void`

Enable/disable components. The enabled components can be updated, while the disabled components cannot be updated.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderNode.enable

#### Defined in

[src/components/ComponentBase.ts:54](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L54)

___

### geometry

• `get` **geometry**(): [`GeometryBase`](GeometryBase.md)

The geometry of the mesh determines its shape

#### Returns

[`GeometryBase`](GeometryBase.md)

#### Overrides

RenderNode.geometry

#### Defined in

[src/components/renderer/MeshRenderer.ts:50](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L50)

• `set` **geometry**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`GeometryBase`](GeometryBase.md) |

#### Returns

`void`

#### Overrides

RenderNode.geometry

#### Defined in

[src/components/renderer/MeshRenderer.ts:55](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L55)

___

### material

• `get` **material**(): `MaterialBase`

material

#### Returns

`MaterialBase`

#### Defined in

[src/components/renderer/MeshRenderer.ts:82](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L82)

• `set` **material**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `MaterialBase` |

#### Returns

`void`

#### Defined in

[src/components/renderer/MeshRenderer.ts:87](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L87)

___

### renderOrder

• `get` **renderOrder**(): `number`

#### Returns

`number`

#### Inherited from

RenderNode.renderOrder

#### Defined in

[src/components/renderer/RenderNode.ts:94](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L94)

• `set` **renderOrder**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderNode.renderOrder

#### Defined in

[src/components/renderer/RenderNode.ts:98](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L98)

___

### rendererMask

• `get` **rendererMask**(): `number`

#### Returns

`number`

#### Inherited from

RenderNode.rendererMask

#### Defined in

[src/components/renderer/RenderNode.ts:132](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L132)

• `set` **rendererMask**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderNode.rendererMask

#### Defined in

[src/components/renderer/RenderNode.ts:136](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L136)

___

### materials

• `get` **materials**(): `MaterialBase`[]

#### Returns

`MaterialBase`[]

#### Inherited from

RenderNode.materials

#### Defined in

[src/components/renderer/RenderNode.ts:140](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L140)

• `set` **materials**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `MaterialBase`[] |

#### Returns

`void`

#### Inherited from

RenderNode.materials

#### Defined in

[src/components/renderer/RenderNode.ts:145](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L145)

___

### castShadow

• `get` **castShadow**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderNode.castShadow

#### Defined in

[src/components/renderer/RenderNode.ts:290](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L290)

• `set` **castShadow**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderNode.castShadow

#### Defined in

[src/components/renderer/RenderNode.ts:295](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L295)

___

### castGI

• `get` **castGI**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderNode.castGI

#### Defined in

[src/components/renderer/RenderNode.ts:300](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L300)

• `set` **castGI**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderNode.castGI

#### Defined in

[src/components/renderer/RenderNode.ts:305](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L305)

___

### castReflection

• `get` **castReflection**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderNode.castReflection

#### Defined in

[src/components/renderer/RenderNode.ts:310](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L310)

• `set` **castReflection**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderNode.castReflection

#### Defined in

[src/components/renderer/RenderNode.ts:314](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L314)

## Methods

### start

▸ **start**(): `void`

#### Returns

`void`

#### Inherited from

RenderNode.start

#### Defined in

[src/components/ComponentBase.ts:113](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L113)

___

### stop

▸ **stop**(): `void`

#### Returns

`void`

#### Inherited from

RenderNode.stop

#### Defined in

[src/components/ComponentBase.ts:114](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L114)

___

### onUpdate

▸ `Optional` **onUpdate**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | [`View3D`](View3D.md) |

#### Returns

`any`

#### Inherited from

RenderNode.onUpdate

#### Defined in

[src/components/ComponentBase.ts:117](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L117)

___

### onLateUpdate

▸ `Optional` **onLateUpdate**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | [`View3D`](View3D.md) |

#### Returns

`any`

#### Inherited from

RenderNode.onLateUpdate

#### Defined in

[src/components/ComponentBase.ts:118](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L118)

___

### onBeforeUpdate

▸ `Optional` **onBeforeUpdate**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | [`View3D`](View3D.md) |

#### Returns

`any`

#### Inherited from

RenderNode.onBeforeUpdate

#### Defined in

[src/components/ComponentBase.ts:119](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L119)

___

### onGraphic

▸ `Optional` **onGraphic**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | [`View3D`](View3D.md) |

#### Returns

`any`

#### Inherited from

RenderNode.onGraphic

#### Defined in

[src/components/ComponentBase.ts:121](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L121)

___

### onParentChange

▸ `Optional` **onParentChange**(`lastParent?`, `currentParent?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `lastParent?` | [`Object3D`](Object3D.md) |
| `currentParent?` | [`Object3D`](Object3D.md) |

#### Returns

`any`

#### Inherited from

RenderNode.onParentChange

#### Defined in

[src/components/ComponentBase.ts:122](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L122)

___

### onEnable

▸ **onEnable**(): `void`

#### Returns

`void`

#### Overrides

RenderNode.onEnable

#### Defined in

[src/components/renderer/MeshRenderer.ts:28](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L28)

___

### onDisable

▸ **onDisable**(): `void`

#### Returns

`void`

#### Overrides

RenderNode.onDisable

#### Defined in

[src/components/renderer/MeshRenderer.ts:32](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L32)

___

### cloneTo

▸ **cloneTo**(`obj`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `obj` | [`Object3D`](Object3D.md) |

#### Returns

`void`

#### Overrides

RenderNode.cloneTo

#### Defined in

[src/components/renderer/MeshRenderer.ts:36](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L36)

___

### copyComponent

▸ **copyComponent**(`from`): [`MeshRenderer`](MeshRenderer.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `from` | [`MeshRenderer`](MeshRenderer.md) |

#### Returns

[`MeshRenderer`](MeshRenderer.md)

#### Overrides

RenderNode.copyComponent

#### Defined in

[src/components/renderer/MeshRenderer.ts:41](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L41)

___

### setMorphInfluence

▸ **setMorphInfluence**(`key`, `value`): `void`

Set deformation animation parameters

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `string` |
| `value` | `number` |

#### Returns

`void`

#### Defined in

[src/components/renderer/MeshRenderer.ts:95](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L95)

___

### setMorphInfluenceIndex

▸ **setMorphInfluenceIndex**(`index`, `value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |
| `value` | `number` |

#### Returns

`void`

#### Defined in

[src/components/renderer/MeshRenderer.ts:104](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L104)

___

### onCompute

▸ **onCompute**(`view`, `command`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view` | [`View3D`](View3D.md) |
| `command` | `GPUCommandEncoder` |

#### Returns

`void`

#### Overrides

RenderNode.onCompute

#### Defined in

[src/components/renderer/MeshRenderer.ts:113](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L113)

___

### destroy

▸ **destroy**(`force?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `force?` | `boolean` |

#### Returns

`void`

#### Overrides

RenderNode.destroy

#### Defined in

[src/components/renderer/MeshRenderer.ts:143](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/MeshRenderer.ts#L143)

___

### init

▸ **init**(): `void`

#### Returns

`void`

#### Inherited from

RenderNode.init

#### Defined in

[src/components/renderer/RenderNode.ts:58](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L58)

___

### attachSceneOctree

▸ **attachSceneOctree**(`octree`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `octree` | [`Octree`](Octree.md) |

#### Returns

`void`

#### Inherited from

RenderNode.attachSceneOctree

#### Defined in

[src/components/renderer/RenderNode.ts:63](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L63)

___

### detachSceneOctree

▸ **detachSceneOctree**(): `void`

#### Returns

`void`

#### Inherited from

RenderNode.detachSceneOctree

#### Defined in

[src/components/renderer/RenderNode.ts:68](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L68)

___

### addMask

▸ **addMask**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | [`RendererMask`](../enums/RendererMask.md) |

#### Returns

`void`

#### Inherited from

RenderNode.addMask

#### Defined in

[src/components/renderer/RenderNode.ts:120](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L120)

___

### removeMask

▸ **removeMask**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | [`RendererMask`](../enums/RendererMask.md) |

#### Returns

`void`

#### Inherited from

RenderNode.removeMask

#### Defined in

[src/components/renderer/RenderNode.ts:124](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L124)

___

### hasMask

▸ **hasMask**(`mask`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | [`RendererMask`](../enums/RendererMask.md) |

#### Returns

`boolean`

#### Inherited from

RenderNode.hasMask

#### Defined in

[src/components/renderer/RenderNode.ts:128](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L128)

___

### addRendererMask

▸ **addRendererMask**(`tag`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `tag` | [`RendererMask`](../enums/RendererMask.md) |

#### Returns

`void`

#### Inherited from

RenderNode.addRendererMask

#### Defined in

[src/components/renderer/RenderNode.ts:176](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L176)

___

### removeRendererMask

▸ **removeRendererMask**(`tag`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `tag` | [`RendererMask`](../enums/RendererMask.md) |

#### Returns

`void`

#### Inherited from

RenderNode.removeRendererMask

#### Defined in

[src/components/renderer/RenderNode.ts:180](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L180)

___

### selfCloneMaterials

▸ **selfCloneMaterials**(`key`): [`MeshRenderer`](MeshRenderer.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `key` | `string` |

#### Returns

[`MeshRenderer`](MeshRenderer.md)

#### Inherited from

RenderNode.selfCloneMaterials

#### Defined in

[src/components/renderer/RenderNode.ts:196](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L196)

___

### renderPass

▸ **renderPass**(`view`, `passType`, `renderContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view` | [`View3D`](View3D.md) |
| `passType` | `RendererType` |
| `renderContext` | [`RenderContext`](RenderContext.md) |

#### Returns

`void`

#### Inherited from

RenderNode.renderPass

#### Defined in

[src/components/renderer/RenderNode.ts:318](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L318)

___

### renderPass2

▸ **renderPass2**(`view`, `passType`, `rendererPassState`, `clusterLightingBuffer`, `encoder`, `useBundle?`): `void`

render pass at passType

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `view` | [`View3D`](View3D.md) | `undefined` |
| `passType` | `RendererType` | `undefined` |
| `rendererPassState` | `RendererPassState` | `undefined` |
| `clusterLightingBuffer` | [`ClusterLightingBuffer`](ClusterLightingBuffer.md) | `undefined` |
| `encoder` | `GPURenderPassEncoder` | `undefined` |
| `useBundle` | `boolean` | `false` |

#### Returns

`void`

#### Inherited from

RenderNode.renderPass2

#### Defined in

[src/components/renderer/RenderNode.ts:371](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L371)

___

### recordRenderPass2

▸ **recordRenderPass2**(`view`, `passType`, `rendererPassState`, `clusterLightingBuffer`, `encoder`, `useBundle?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `view` | [`View3D`](View3D.md) | `undefined` |
| `passType` | `RendererType` | `undefined` |
| `rendererPassState` | `RendererPassState` | `undefined` |
| `clusterLightingBuffer` | [`ClusterLightingBuffer`](ClusterLightingBuffer.md) | `undefined` |
| `encoder` | `GPURenderPassEncoder` | `undefined` |
| `useBundle` | `boolean` | `false` |

#### Returns

`void`

#### Inherited from

RenderNode.recordRenderPass2

#### Defined in

[src/components/renderer/RenderNode.ts:416](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L416)

___

### beforeDestroy

▸ **beforeDestroy**(`force?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `force?` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderNode.beforeDestroy

#### Defined in

[src/components/renderer/RenderNode.ts:527](https://github.com/Orillusion/orillusion/blob/main/src/components/renderer/RenderNode.ts#L527)
