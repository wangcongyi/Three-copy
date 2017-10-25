## scene 中最常用的方法和属性
### 具体代码请参照 [chapter-2.html](https://github.com/wangcongyi/Three-copy/blob/master/new/chapter-2.html) 的代码


```js

  const scene = new THREE.Scene();
  
  scene.add(object)
  //用于向场景中添加对象。使用该方法还可以创建对象组
  
  scene.children
  // 返回场景中所有对象列表，包括摄像机和光源
  
  scene.getObjectByName(name,recursive)
  // 在创建对象时候可以指定唯一的标示 name，使用该方法
  // 可以查找特定名称的对象，当参数 recursive 为 false 时
  // 在调用者子元素上查找，true 在调用者后代对象上查找
  
  scene.remove(object)
  // 将对象在场景中移除
  
  scene.traverse(func)
  // 遍历调用者和其所有后代，调用参数 func 的方法
  
  
  scene.fog
  // 为场景增加雾化效果
  
  scene.overrideMaterial
  // 强制场景中所有物体使用相同的材质
  



```