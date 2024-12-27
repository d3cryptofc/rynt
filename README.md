<p align="center">
  <img src="https://raw.githubusercontent.com/gist/d3cryptofc/c52a2565ed2194809ccd3896ca4ed772/raw/fb732058e24697e9ca13f7946839e3ce9e7e0812/rynt.svg" width="500"><br><br>
  <b>Type Hint Remover Tool for Python</b><br>
  For what type hints in production? Avoid unnecessary imports to optimize your code.<br><br>
</p>


```diff
 a = 1
-b: int
-c: int = 1
+c = 1
 
 
-async def function(a, b: int, c = 1, d: int = 1, *e: int, **f: int) -> int:
+async def function(a, b, c = 1, d = 1, *e, **f):
     a = 1
-    b: int
-    c: int = 1
+    c = 1
 
     if _:
         a = 1
-        b: int
-        c: int = 1
+        c = 1
 
     with _:
         a = 1
-        b: int
-        c: int = 1
-    
+        c = 1
+
     for _ in __:
         a = 1
-        b: int
-        c: int = 1
+        c = 1
 
     while _:
         a = 1
-        b: int
-        c: int = 1
+        c = 1
 
     class Subclass:
         a = 1
-        b: int
-        c: int = 1
+        c = 1
 
-        def method(self, a, b: int, c = 1, d: int = 1, *e: int, **f: int) -> int:
+        def method(self, a, b, c = 1, d = 1, *e, **f):
             a = 1
-            b: int
-            c: int = 1
+            c = 1
+
```
