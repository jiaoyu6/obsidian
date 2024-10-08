Controller方法没有加@ResponseBody导致api访问404
```kotlin
}
```

在使用@Controller注解编写控制层的接口时，如果方法的返回值是String类型，而且又没有使用 @ResponseBody 注解，那么 spring mvc 框架则会认为该方法的返回值就是 ModelAndViewer 对象，相当于是一个待跳转的页面，要么是jsp，要么是Freemarker等等。

可想而知，spring mvc是肯定找不到如代码中的接口那样的页面的，所有导致跳转的时候找不到这个 viewer ，就报404了

  