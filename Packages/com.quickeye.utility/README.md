Collection of small useful classes.

### `Singleton<T>`

`MonoBehaviour` Singleton implementation.

* Allows for prefab instantiation together with `SingletonAssetAttribute`
* Takes into account some common problems of many singleton implementations that are out there.

### `Container` and `PoolContainer`

A serializable object that holds a prefab and a `Transform` reference, implements `IList<T>`.
`AddNew` method creates a new instance of prefab inside the transform. Because of `IList<T>`, it functions as a
collection with additional behavior of easy object instantiation.
`PoolContainer` has the same interface but uses object pooling. Cuts much of the boilerplate code with UI scripting.

### `GameObjectPool`

Object pool pattern implementation with Unity specific API.

* Serializable, can be configured from editor.
* Prototype as prefab.
* Configurable transform parent.