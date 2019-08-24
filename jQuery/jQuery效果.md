## jQuery效果

- jQuery隐藏/显示

  ```
  $(selector).hide(speed,callback);

  $(selector).show(speed,callback);
  
  $(selector).toggle(speed,callback);
  ```
  speed：隐藏/显示的速度；slow/fast/毫秒数;
  
  callback：隐藏/显示完成后执行的函数名称。
  
  toggle()切换hide()和show()方法
  
  ***
  
- jQuery淡入/淡出

  ```
  $(selector).fadeIn(speed,callback);
  
  $(selector).fadeOut(speed,callback);
  
  $(selector).fadeToggle(speed,callback);
  
  $(selector).fadeTo(speed,opacity,callback);
  ```
  adeTo() 方法中必需的 opacity 参数将淡入淡出效果设置为给定的不透明度（值介于 0 与 1 之间）
  
- jQuery滑动

  ```
  $(selector).slideDown(speed,callback);
  
  $(selector).slideUp(speed,callback);
  
  $(selector).slideToggle(speed,callback);
  
  ```
- jQuery动画

  ```
  $(selector).animate({params},speed,callback);
  ```
  params：必需，定义形成动画的CSS属性。  
  
  操作多个属性用“，”分隔；  
  
  必须使用 Camel 标记法书写所有的属性名，如“padding-left”要写成“paddingLeft”；  
  
  使用相对值，如“height:'+=150px'”；  
  
  还可以把属性的动画值设置为 "show"、"hide" 或 "toggle"等预定义的值，如“height:'toggle'”；  
  
  编写多个 animate() 调用，jQuery 会逐一运行这些 animate 调用。
  
- jQuery停止动画

  ```
  $(selector).stop(stopAll,goToEnd);
  ```
  stopAll:可选，默认是 false，即仅停止活动的动画，允许任何排入队列的动画向后执行；
  
   goToEnd：可选，规定是否立即完成当前动画，默认是 false。
   
 - jQuery chaining
 
  Chaining 允许在一条语句中实现多个jQuery方法（在相同的元素上），例如：
  ```
  $("#p1").css("color","red").slideUp(2000).slideDown(2000);
  ```
  "p1" 元素首先会变为红色，然后向上滑动，然后向下滑动。
  
  
