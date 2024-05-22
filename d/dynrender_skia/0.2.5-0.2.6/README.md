# Comparing `tmp/dynrender_skia-0.2.5.tar.gz` & `tmp/dynrender_skia-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynrender_skia-0.2.5.tar", max compression
+gzip compressed data, was "dynrender_skia-0.2.6.tar", last modified: Wed May 22 12:48:16 2024, max compression
```

## Comparing `dynrender_skia-0.2.5.tar` & `dynrender_skia-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0    35149 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/LICENSE
--rw-r--r--   0        0        0     1504 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/README.md
--rw-r--r--   0        0        0     2225 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/Core.py
--rw-r--r--   0        0        0    18382 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynAdditional.py
--rw-r--r--   0        0        0     5499 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynConfig.py
--rw-r--r--   0        0        0    11240 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynHeader.py
--rw-r--r--   0        0        0    33217 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynMajor.py
--rw-r--r--   0        0        0     1209 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynRepost.py
--rw-r--r--   0        0        0      849 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynStyle.py
--rw-r--r--   0        0        0    12798 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynText.py
--rw-r--r--   0        0        0     4065 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/DynTools.py
--rw-r--r--   0        0        0   341424 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/Static.zip
--rw-r--r--   0        0        0        0 2023-11-18 14:07:15.897371 dynrender_skia-0.2.5/dynrender_skia/__init__.py
--rw-r--r--   0        0        0      458 2023-11-18 14:07:15.901371 dynrender_skia-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 dynrender_skia-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1824 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/README.md
+-rw-r--r--   0        0        0     2243 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/Core.py
+-rw-r--r--   0        0        0    19204 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynAdditional.py
+-rw-r--r--   0        0        0     5538 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynConfig.py
+-rw-r--r--   0        0        0    11234 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynHeader.py
+-rw-r--r--   0        0        0    35404 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynMajor.py
+-rw-r--r--   0        0        0     1187 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynRepost.py
+-rw-r--r--   0        0        0      825 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynStyle.py
+-rw-r--r--   0        0        0    12505 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynText.py
+-rw-r--r--   0        0        0     4998 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/DynTools.py
+-rw-r--r--   0        0        0   341424 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/Static.zip
+-rw-r--r--   0        0        0        0 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/dynrender_skia/__init__.py
+-rw-r--r--   0        0        0     1940 2024-05-22 12:48:16.107724 dynrender_skia-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0     5777 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/tests/res/bilibili.png
+-rw-r--r--   0        0        0     7789 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/tests/res/message.json
+-rw-r--r--   0        0        0      574 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/tests/test_dynrender_run.py
+-rw-r--r--   0        0        0     4814 2024-05-22 12:48:01.559563 dynrender_skia-0.2.6/tests/test_tools.py
+-rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 dynrender_skia-0.2.6/PKG-INFO
```

### Comparing `dynrender_skia-0.2.5/LICENSE` & `dynrender_skia-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.2.5/README.md` & `dynrender_skia-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DynRender-skia
 使用skia渲染BiliBili动态
-
+更新页面效果的优先级会很低
 # 注意
 
 Linux用户在导入skia-python包时可能会遇到以下报错
 ```bash
 libGL.so.1: cannot open shared object file: No such file or directory
 ```
 ## 解决方法
@@ -40,28 +40,41 @@
 import httpx
 import asyncio
 import skia
 from dynrender_skia.Core import DynRender
 from dynamicadaptor.DynamicConversion import formate_message
 
 
+# 定义异步函数，用于执行Web测试
 async def web_test():
     dyn_id = "440646043801479846"
     url = f"https://api.bilibili.com/x/polymer/web-dynamic/v1/detail?timezone_offset=-480&id={dyn_id}&features=itemOpusStyle"
     headers = {
         "referer": f"https://t.bilibili.com/{dyn_id}",
         "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
     }
+
+    # 发起HTTP请求并解析JSON响应
     message_json = httpx.get(url, headers=headers).json()
 
+    # 格式化消息数据
     message_formate = await formate_message("web", message_json["data"]["item"])
+
+    # 使用DynRender执行动态渲染
     img = await DynRender().run(message_formate)
+
+    # 将渲染后的图像转换为Skia Image对象
     img = skia.Image.fromarray(img, colorType=skia.ColorType.kRGBA_8888_ColorType)
+
+    # 保存图像为PNG文件
     img.save("1.png")
 
+
+# 当文件作为主程序执行时
 if __name__ == "__main__":
     asyncio.run(web_test())
 
+
 ```
 
 ## 效果展示
 ![示例图片](https://i0.hdslb.com/bfs/new_dyn/a1fae2ca072ef96bc66dc12ea6de569c37815472.png)
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/Core.py` & `dynrender_skia-0.2.6/dynrender_skia/Core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 @File    :   Core.py
 @Time    :   2023/07/13 15:21:46
-@Author  :   Polyisoprene 
+@Author  :   Polyisoprene
 @Version :   1.0
 @Desc    :   None
-'''
+"""
+
 import asyncio
+from typing import Optional
 
 from dynamicadaptor.Message import RenderMessage
 
 from .DynAdditional import BiliAdditional
 from .DynConfig import MakeStaticFile, SetDynStyle
 from .DynHeader import BiliHeader, Footer
 from .DynMajor import BiliMajor
 from .DynRepost import BiliRepost
 from .DynText import BiliText
 from .DynTools import merge_pictures
 
 
 class DynRender:
-    def __init__(self, font_family: str = "Noto Sans CJK SC",
-                 emoji_font_family: str = "Noto Color Emoji",
-                 font_style: str = "Normal",
-                 static_path: str = None) -> None:
+    def __init__(
+        self,
+        font_family: str = "Noto Sans SC",
+        emoji_font_family: str = "Noto Color Emoji",
+        font_style: str = "Normal",
+        static_path: Optional[str] = None,
+    ) -> None:
         """create static file and set font family and font style
 
         Args:
             font_family (str, optional): font family name like "Noto Sans CJK SC". Defaults to "Noto Sans CJK SC".
-            emoji_font_family (str, optional):emoji font family name like "Noto Color Emoji". Defaults to "Noto Sans CJK SC".
+            emoji_font_family (str, optional):emoji font family name like "Noto Color Emoji".
+            Defaults to "Noto Sans CJK SC".
             font_style (str, optional): font style like "Normal、Bold、Italic、BoldItalic". Defaults to "Normal".
             static_path (str, optional): static file path,must be absolute path. Defaults to None.
         """
         self.static_path = MakeStaticFile(static_path).check_cache_file
         self.style = SetDynStyle(font_family, emoji_font_family, font_style).set_style
 
     async def run(self, message: RenderMessage):
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynAdditional.py` & `dynrender_skia-0.2.6/dynrender_skia/DynAdditional.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,59 +14,65 @@
 
 class AbstractAdditional(ABC):
     def __init__(self, src_path: str, style: PolyStyle, additional: Additional) -> None:
         self.style = style
         self.additional = additional
         self.src_path = src_path
         self.canvas = None
-        self.text_font = skia.Font(skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
-                                   self.style.font.font_size.text)
+        self.text_font = skia.Font(
+            skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
+            self.style.font.font_size.text,
+        )
         self.emoji_font = skia.Font(
-            skia.Typeface.MakeFromName(
-                self.style.font.emoji_font_family, self.style.font.font_style),
-            self.style.font.font_size.text)
+            skia.Typeface.MakeFromName(self.style.font.emoji_font_family, self.style.font.font_style),
+            self.style.font.font_size.text,
+        )
 
     @abstractmethod
     async def run(self, repost: bool) -> Optional[np.ndarray]:
         pass
 
     async def make_badge(self, badge: str, font_size: int, pos: tuple, img_size: tuple, text_pos: tuple):
         self.text_font.setSize(font_size)
         surface = skia.Surface(*img_size)
         canvas = surface.getCanvas()
         canvas.clear(skia.Color(*self.style.color.font_color.name_big_vip))
         blob = skia.TextBlob(badge, self.text_font)
         paint = skia.Paint(AntiAlias=True, Color=skia.Color4f.kWhite)
         canvas.drawTextBlob(blob, text_pos[0], text_pos[1], paint)
-        tag_img = skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                       colorType=skia.ColorType.kRGBA_8888_ColorType)
+        tag_img = skia.Image.fromarray(
+            canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            colorType=skia.ColorType.kRGBA_8888_ColorType,
+        )
         tag_img = await self.make_round_cornor(tag_img, 10)
         await paste(self.canvas, tag_img, pos)
 
     async def make_round_cornor(self, img, corner: int):
         surface = skia.Surface(img.width(), img.height())
         mask = surface.getCanvas()
         paint = skia.Paint(
             Style=skia.Paint.kFill_Style,
             Color=skia.Color(255, 255, 255, 255),
-            AntiAlias=True)
+            AntiAlias=True,
+        )
         rect = skia.Rect.MakeXYWH(0, 0, img.width(), img.height())
         mask.drawRoundRect(rect, corner, corner, paint)
-        image_array = np.bitwise_and(img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                     mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
+        image_array = np.bitwise_and(
+            img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+        )
         return skia.Image.fromarray(image_array, colorType=skia.ColorType.kRGBA_8888_ColorType)
 
     async def draw_shadow(self, canvas, pos: tuple, corner: int, bg_color):
         x, y, width, height = pos
         rec = skia.Rect.MakeXYWH(x, y, width, height)
         paint = skia.Paint(
             Color=skia.Color(*bg_color),
             AntiAlias=True,
-            ImageFilter=skia.ImageFilters.DropShadow(
-                0, 0, 10, 10, skia.Color(120, 120, 120))
+            ImageFilter=skia.ImageFilters.DropShadow(0, 0, 10, 10, skia.Color(120, 120, 120)),
         )
         if corner != 0:
             canvas.drawRoundRect(rec, corner, corner, paint)
         else:
             canvas.drawRect(rec, paint)
 
 
@@ -95,15 +101,14 @@
                 return None
         except Exception as e:
             logger.exception(e)
             return None
 
 
 class DynAddReserve(AbstractAdditional):
-
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 225)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.draw_shadow(self.canvas, (35, 20, 1010, 185), 15, background_color)
@@ -113,37 +118,60 @@
         except Exception as e:
             logger.exception(e)
             return None
 
     async def make_desc(self):
         draw = DrawText(self.style)
         if self.additional.reserve.desc3 is not None:
-            await draw.draw_text(self.canvas, self.additional.reserve.title, self.style.font.font_size.time,
-                                 (75, 70, 740, 70, 0), self.style.color.font_color.text)
+            await draw.draw_text(
+                self.canvas,
+                self.additional.reserve.title,
+                self.style.font.font_size.time,
+                (75, 70, 740, 70, 0),
+                self.style.color.font_color.text,
+            )
             desc_1 = f"{self.additional.reserve.desc1.text}  {self.additional.reserve.desc2.text}"
-            await draw.draw_text(self.canvas, desc_1, self.style.font.font_size.title,
-                                 (75, 120, 810, 120, 0), self.style.color.font_color.sub_title)
-
-            await draw.draw_text(self.canvas, self.additional.reserve.desc3.text, self.style.font.font_size.title,
-                                 (105, 170, 810, 170, 0), self.style.color.font_color.rich_text)
+            await draw.draw_text(
+                self.canvas,
+                desc_1,
+                self.style.font.font_size.title,
+                (75, 120, 810, 120, 0),
+                self.style.color.font_color.sub_title,
+            )
+
+            await draw.draw_text(
+                self.canvas,
+                self.additional.reserve.desc3.text,
+                self.style.font.font_size.title,
+                (105, 170, 810, 170, 0),
+                self.style.color.font_color.rich_text,
+            )
 
-            lottery_img = skia.Image.open(
-                path.join(self.src_path, "lottery.png")).resize(40, 40)
+            lottery_img = skia.Image.open(path.join(self.src_path, "lottery.png")).resize(40, 40)
             await paste(self.canvas, lottery_img, (65, 138))
         else:
-            await draw.draw_text(self.canvas, self.additional.reserve.title, self.style.font.font_size.time,
-                                 (75, 100, 740, 100, 0), self.style.color.font_color.text)
+            await draw.draw_text(
+                self.canvas,
+                self.additional.reserve.title,
+                self.style.font.font_size.time,
+                (75, 100, 740, 100, 0),
+                self.style.color.font_color.text,
+            )
 
             desc_1 = f"{self.additional.reserve.desc1.text}  {self.additional.reserve.desc2.text}"
-            await draw.draw_text(self.canvas, desc_1, self.style.font.font_size.title,
-                                 (75, 160, 810, 160, 0), self.style.color.font_color.sub_title)
+            await draw.draw_text(
+                self.canvas,
+                desc_1,
+                self.style.font.font_size.title,
+                (75, 160, 810, 160, 0),
+                self.style.color.font_color.sub_title,
+            )
 
 
 class DynAddUpOwerLottery(AbstractAdditional):
-
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 225)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.draw_shadow(self.canvas, (35, 20, 1010, 185), 15, background_color)
@@ -152,70 +180,97 @@
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
     async def make_desc(self):
         draw = DrawText(self.style)
-        await draw.draw_text(self.canvas, self.additional.upower_lottery.title, self.style.font.font_size.time,
-                             (75, 100, 740, 100, 0), self.style.color.font_color.text)
+        await draw.draw_text(
+            self.canvas,
+            self.additional.upower_lottery.title,
+            self.style.font.font_size.time,
+            (75, 100, 740, 100, 0),
+            self.style.color.font_color.text,
+        )
 
-        await draw.draw_text(self.canvas, self.additional.upower_lottery.desc.text, self.style.font.font_size.title,
-                             (105, 160, 810, 160, 0), self.style.color.font_color.rich_text)
-        lottery_img = skia.Image.open(
-            path.join(self.src_path, "lottery.png")).resize(40, 40)
+        await draw.draw_text(
+            self.canvas,
+            self.additional.upower_lottery.desc.text,
+            self.style.font.font_size.title,
+            (105, 160, 810, 160, 0),
+            self.style.color.font_color.rich_text,
+        )
+        lottery_img = skia.Image.open(path.join(self.src_path, "lottery.png")).resize(40, 40)
         await paste(self.canvas, lottery_img, (65, 128))
 
 
 class DynAddGoods(AbstractAdditional):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 310)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.draw_shadow(self.canvas, (35, 50, 1010, 240), 15, background_color)
             await self.make_cover()
             await self.make_title_desc()
-            await DrawText(self.style).draw_text(self.canvas, self.additional.goods.head_text,
-                                                 self.style.font.font_size.sub_title, (
-                                                     45, 30, 1010, 80, 0),
-                                                 self.style.color.font_color.sub_title)
-            await self.make_badge("去看看", self.style.font.font_size.time, (860, 125), (155, 75), (25, 50))
+            await DrawText(self.style).draw_text(
+                self.canvas,
+                self.additional.goods.head_text,
+                self.style.font.font_size.sub_title,
+                (45, 30, 1010, 80, 0),
+                self.style.color.font_color.sub_title,
+            )
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
     async def make_cover(self):
         url_list = []
         for i in self.additional.goods.items:
-            url = re.sub("@(\d+)h_(\d+)w\S+", "", i.cover)
+            url = re.sub(r"@(\d+)h_(\d+)w\S+", "", i.cover)
             url_list.append(f"{url}@160w_160h_1c.webp")
         covers = await get_pictures(url_list, (190, 190))
         if len(covers) > 1:
             for i, j in enumerate(covers):
                 x = 45 + i * 200
                 if x > 1000:
                     break
                 await paste(self.canvas, await self.make_round_cornor(j, 10), (x, 75))
         else:
             await paste(self.canvas, await self.make_round_cornor(covers[0], 10), (60, 75))
+            await self.make_badge(
+                "去看看",
+                self.style.font.font_size.time,
+                (860, 125),
+                (155, 75),
+                (25, 50),
+            )
 
     async def make_title_desc(self):
         if len(self.additional.goods.items) > 1:
             return
         draw = DrawText(self.style)
-        await draw.draw_text(self.canvas, self.additional.goods.items[0].name, self.style.font.font_size.title,
-                             (275, 140, 800, 140, 0), self.style.color.font_color.text)
+        await draw.draw_text(
+            self.canvas,
+            self.additional.goods.items[0].name,
+            self.style.font.font_size.title,
+            (275, 140, 800, 140, 0),
+            self.style.color.font_color.text,
+        )
 
         price = f"{self.additional.goods.items[0].price}起"
-        await draw.draw_text(self.canvas, price, self.style.font.font_size.title,
-                             (295, 210, 800, 210, 0), self.style.color.font_color.rich_text)
+        await draw.draw_text(
+            self.canvas,
+            price,
+            self.style.font.font_size.title,
+            (295, 210, 800, 210, 0),
+            self.style.color.font_color.rich_text,
+        )
 
 
 class DynAddUgc(AbstractAdditional):
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 280)
         self.canvas = surface.getCanvas()
@@ -234,36 +289,50 @@
 
     async def make_cover(self):
         cover = await get_pictures(f"{self.additional.ugc.cover}@340w_195h_1c.webp")
         await paste(self.canvas, await self.make_round_cornor(cover, 10), (60, 45))
 
     async def make_title_desc(self):
         draw = DrawText(self.style)
-        await draw.draw_text(self.canvas, self.additional.ugc.title, self.style.font.font_size.title,
-                             (430, 90, 990, 140, int(self.style.font.font_size.time * 1.3)),
-                             self.style.color.font_color.text)
-        await draw.draw_text(self.canvas, self.additional.ugc.desc_second, self.style.font.font_size.title,
-                             (430, 220, 950, 220, 0), self.style.color.font_color.sub_title)
+        await draw.draw_text(
+            self.canvas,
+            self.additional.ugc.title,
+            self.style.font.font_size.title,
+            (430, 90, 990, 140, int(self.style.font.font_size.time * 1.3)),
+            self.style.color.font_color.text,
+        )
+        await draw.draw_text(
+            self.canvas,
+            self.additional.ugc.desc_second,
+            self.style.font.font_size.title,
+            (430, 220, 950, 220, 0),
+            self.style.color.font_color.sub_title,
+        )
 
     async def make_sub_tag(self):
         self.text_font.setSize(self.style.font.font_size.sub_title)
         size = self.text_font.measureText(self.additional.ugc.duration)
         surface = skia.Surface(int(size + 20), int(self.text_font.getSize() + 20))
         canvas = surface.getCanvas()
         canvas.clear(skia.Color(0, 0, 0, 150))
         blob = skia.TextBlob(self.additional.ugc.duration, self.text_font)
         paint = skia.Paint(AntiAlias=True, Color=skia.Color4f.kWhite)
         canvas.drawTextBlob(blob, 10, int(self.text_font.getSize() + 5), paint)
-        sub_tag_img = skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                           colorType=skia.ColorType.kRGBA_8888_ColorType)
-        await paste(self.canvas, await self.make_round_cornor(sub_tag_img, 10), (400 - sub_tag_img.width() - 15, 190))
+        sub_tag_img = skia.Image.fromarray(
+            canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            colorType=skia.ColorType.kRGBA_8888_ColorType,
+        )
+        await paste(
+            self.canvas,
+            await self.make_round_cornor(sub_tag_img, 10),
+            (400 - sub_tag_img.width() - 15, 190),
+        )
 
 
 class DynAddVote(AbstractAdditional):
-
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 280)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.draw_shadow(self.canvas, (35, 20, 1010, 240), 15, background_color)
@@ -280,39 +349,51 @@
 
     async def make_cover(self):
         cover = skia.Image.open(fp=path.join(self.src_path, "vote_icon.png")).resize(195, 195)
         await paste(self.canvas, await self.make_round_cornor(cover, 10), (60, 45))
 
     async def make_title_desc(self):
         draw = DrawText(self.style)
-        await draw.draw_text(self.canvas, self.additional.vote.desc, self.style.font.font_size.text,
-                             (280, 110, 810, 110, 0),
-                             self.style.color.font_color.text)
+        await draw.draw_text(
+            self.canvas,
+            self.additional.vote.desc,
+            self.style.font.font_size.text,
+            (280, 110, 810, 110, 0),
+            self.style.color.font_color.text,
+        )
         if self.additional.vote.join_num is None:
             join_num = "0人参与"
         else:
             join_num = f"{self.additional.vote.join_num}人参与"
 
-        await draw.draw_text(self.canvas, join_num, self.style.font.font_size.time,
-                             (280, 190, 810, 190, 0), self.style.color.font_color.sub_title)
+        await draw.draw_text(
+            self.canvas,
+            join_num,
+            self.style.font.font_size.time,
+            (280, 190, 810, 190, 0),
+            self.style.color.font_color.sub_title,
+        )
 
 
 class DynAddCommon(AbstractAdditional):
-
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 340)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.draw_shadow(self.canvas, (35, 80, 1010, 245), 15, background_color)
 
-            await DrawText(self.style).draw_text(self.canvas, self.additional.common.head_text,
-                                                 self.style.font.font_size.title, (50, 50, 1010, 90, 0),
-                                                 self.style.color.font_color.sub_title)
+            await DrawText(self.style).draw_text(
+                self.canvas,
+                self.additional.common.head_text,
+                self.style.font.font_size.title,
+                (50, 50, 1010, 90, 0),
+                self.style.color.font_color.sub_title,
+            )
 
             rec = skia.Rect.MakeXYWH(35, 80, 1010, 240)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
 
             await self.make_cover()
             await self.select_badge()
             await self.select_badge()
@@ -321,55 +402,75 @@
 
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
     async def make_cover(self):
-        if self.additional.common.sub_type in {'decoration', 'game'}:
+        if self.additional.common.sub_type in {"decoration", "game"}:
             cover_url = f"{self.additional.common.cover}@190w_190h_1c.webp"
             cover = await get_pictures(cover_url, (190, 190))
         else:
             cover_url = f"{self.additional.common.cover}@145w_195h_1c.webp"
             cover = await get_pictures(cover_url, (145, 195))
         await paste(self.canvas, await self.make_round_cornor(cover, 15), (60, 110))
 
     async def make_title(self):
         if self.additional.common.desc2:
             y = 150
         else:
             y = 180
-        if self.additional.common.sub_type in {'decoration', 'game'}:
+        if self.additional.common.sub_type in {"decoration", "game"}:
             x = 280
         else:
             x = 250
-        await DrawText(self.style).draw_text(self.canvas, self.additional.common.title, self.style.font.font_size.text,
-                                             (x, y, 780, y, 0), self.style.color.font_color.text)
+        await DrawText(self.style).draw_text(
+            self.canvas,
+            self.additional.common.title,
+            self.style.font.font_size.text,
+            (x, y, 780, y, 0),
+            self.style.color.font_color.text,
+        )
 
     async def make_desc(self):
         draw = DrawText(self.style)
-        if self.additional.common.sub_type in {'decoration', 'game'}:
+        if self.additional.common.sub_type in {"decoration", "game"}:
             x = 280
         else:
             x = 250
         if self.additional.common.desc2:
-            await draw.draw_text(self.canvas, self.additional.common.desc1, self.style.font.font_size.title,
-                                 (x, 220, 780, 160, 0), self.style.color.font_color.sub_title)
-
-            await draw.draw_text(self.canvas, self.additional.common.desc2, self.style.font.font_size.title,
-                                 (x, 285, 780, 225, 0), self.style.color.font_color.sub_title)
+            await draw.draw_text(
+                self.canvas,
+                self.additional.common.desc1,
+                self.style.font.font_size.title,
+                (x, 220, 780, 160, 0),
+                self.style.color.font_color.sub_title,
+            )
+
+            await draw.draw_text(
+                self.canvas,
+                self.additional.common.desc2,
+                self.style.font.font_size.title,
+                (x, 285, 780, 225, 0),
+                self.style.color.font_color.sub_title,
+            )
         else:
-            await draw.draw_text(self.canvas, self.additional.common.desc1, self.style.font.font_size.title,
-                                 (x, 250, 780, 190, 0), self.style.color.font_color.sub_title)
+            await draw.draw_text(
+                self.canvas,
+                self.additional.common.desc1,
+                self.style.font.font_size.title,
+                (x, 250, 780, 190, 0),
+                self.style.color.font_color.sub_title,
+            )
 
     async def select_badge(self):
         badge_text_map = {
             "pugv": "去试看",
             "ogv": "去看看",
             "manga": "去追漫",
             "decoration": "去看看",
-            "game": "进入"
+            "game": "进入",
         }
         badge_text = badge_text_map.get(self.additional.common.sub_type, "去看看")
         size = self.text_font.measureText(badge_text)
         x = int((155 - size) / 2)
         await self.make_badge(badge_text, self.style.font.font_size.time, (860, 165), (155, 75), (x, 50))
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynConfig.py` & `dynrender_skia-0.2.6/dynrender_skia/DynConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# -*- coding: utf-8 -*-
 """
 @File    :   DynConfig.py
 @Time    :   2023/07/13 14:20:02
-@Author  :   Polyisoprene 
+@Author  :   Polyisoprene
 @Version :   1.0
 @Desc    :   None
 """
+
 import json
 from os import getcwd, makedirs, path
 from typing import Optional
 from zipfile import ZipFile
 
 from loguru import logger
 
 try:
     import skia
 except ImportError as e:
     logger.error(e)
     logger.warning(
         "Missing dependent files \n\n please install dependence: \n\n ---------------------------------------\n\n "
         "Ubuntu: apt install libgl1-mesa-glx \n\n ArchLinux: pacman -S libgl \n\n Centos: yum install mesa-libGL -y "
-        "\n\n---------------------------------------")
+        "\n\n---------------------------------------"
+    )
 from .DynStyle import PolyStyle
 
 
 class MakeStaticFile:
     def __init__(self, data_path: Optional[str] = None) -> None:
         self.data_path: str = data_path
 
@@ -43,29 +44,29 @@
             # 如果不存在静态目录将自带的压缩文件解压过去
             if not path.exists(static_path):
                 logger.info("未检测到static目录")
                 self.unzip_file(
                     "用户未传入data路径,将在程序运行目录创建static目录",
                     "创建static目录中...",
                     current_dir,
-                    program_running_path
+                    program_running_path,
                 )
                 logger.info("static目录创建成功")
         else:
             # 设置静态文件的目录
             static_path = path.join(self.data_path, "Static")
             if not path.exists(self.data_path):
                 # 如果data_path不存在创建这个目录
                 makedirs(self.data_path)
             if not path.exists(static_path):
                 self.unzip_file(
                     "未检测到static目录",
                     "使用用户传入路径创建static目录中...",
                     current_dir,
-                    self.data_path
+                    self.data_path,
                 )
                 logger.info("static目录创建成功")
         font_cache_path = path.join(static_path, "font_family.json")
         if not path.exists(font_cache_path):
             logger.info("创建系统安装的所有字体的名称列表文件")
             font_list = list(skia.FontMgr())
             with open(font_cache_path, "w") as f:
@@ -104,40 +105,44 @@
                 "font_color": {
                     "text": (0, 0, 0, 255),
                     "sub_title": (153, 162, 170, 255),
                     "title": (0, 0, 0, 255),
                     "name_big_vip": (251, 107, 148, 255),
                     "name_small_vip": (60, 232, 78, 255),
                     "rich_text": (0, 161, 214, 255),
-                    "white": (255, 255, 255, 255)
+                    "white": (255, 255, 255, 255),
                 },
                 "background": {
                     "normal": (255, 255, 255, 255),
                     "repost": (241, 242, 243, 255),
-                    "border": (229, 233, 239, 255)
-                }
-
+                    "border": (229, 233, 239, 255),
+                },
             },
             "font": {
                 "font_family": self.font_family,
                 "emoji_font_family": self.emoji_font_family,
                 "font_style": self.get_font_style(),
                 "font_size": {
                     "name": 45,
                     "text": 40,
                     "time": 35,
                     "title": 30,
-                    "sub_title": 20
-                }
-            }
+                    "sub_title": 20,
+                },
+            },
         }
 
         return PolyStyle(**cfg_obj)
 
     def get_font_style(self):
-        style_map = {"Normal": skia.FontStyle().Normal(), "Bold": skia.FontStyle().Bold(
-        ), "Italic": skia.FontStyle().Italic(), "BoldItalic": skia.FontStyle().BoldItalic()}
+        style_map = {
+            "Normal": skia.FontStyle().Normal(),
+            "Bold": skia.FontStyle().Bold(),
+            "Italic": skia.FontStyle().Italic(),
+            "BoldItalic": skia.FontStyle().BoldItalic(),
+        }
         return style_map.get(self.font_style, skia.FontStyle().Normal())
 
+
 # if __name__ == "__main__":
 #     a = SetDynStyle("Noto Sans CJK SC","Normal").set_style
 #     print(a.color.backgroud.repost)
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynHeader.py` & `dynrender_skia-0.2.6/dynrender_skia/DynHeader.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 
     async def run(self, header_message: Head) -> Optional[np.ndarray]:
         try:
             self.message = header_message
             surface = skia.Surface(1080, 400)
             self.canvas = surface.getCanvas()
             self.canvas.clear(skia.Color(*self.style.color.background.normal))
-            result = await asyncio.gather(self.paste_logo(),
-                                          self.draw_name(),
-                                          self.draw_pub_time(),
-                                          self.get_face_and_pendant(True),
-                                          self.get_face_and_pendant()
-                                          )
+            result = await asyncio.gather(
+                self.paste_logo(),
+                self.draw_name(),
+                self.draw_pub_time(),
+                self.get_face_and_pendant(True),
+                self.get_face_and_pendant(),
+            )
             await self.past_face()
             await self.paste_pendant(result[4])
             await self.paste_vip()
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception:
             logger.exception("Error")
             return None
@@ -72,70 +73,86 @@
     async def past_face(self):
         face = await self.get_face_and_pendant(True)
         if face:
             face = await self.circle_face(face, 120)
             await self.paste(face, (45, 245))
 
     async def get_face_and_pendant(self, img_type: bool = False):
-
         if img_type:
             img_name = f"{self.message.mid}.webp"
             img_url = f"{self.message.face}@240w_240h_1c_1s.webp"
             img_path = path.join(self.face_path, img_name)
         elif self.message.pendant and self.message.pendant.image:
-
             img_name = f"{self.message.pendant.pid}.png"
             img_url = f"{self.message.pendant.image}@360w_360h.webp"
             img_path = path.join(self.pendant_path, img_name)
         else:
             return None
         if path.exists(img_path):
             if time() - int(path.getmtime(img_path)) <= 43200:
                 return skia.Image.open(img_path)
         img = await get_pictures(img_url)
         if img is not None:
             img.save(img_path)
             return img
         return None
 
-    async def circle_face(self, img, size):
-        surface = skia.Surface(img.dimensions().width(),
-                               img.dimensions().height())
+    @staticmethod
+    async def circle_face(img: skia.Image, size: int) -> object:
+        surface = skia.Surface(img.dimensions().width(), img.dimensions().height())
         mask = surface.getCanvas()
         paint = skia.Paint(
             Style=skia.Paint.kFill_Style,
             Color=skia.Color(255, 255, 255, 255),
-            AntiAlias=True)
+            AntiAlias=True,
+        )
         radius = int(img.dimensions().width() / 2)
         mask.drawCircle(radius, radius, radius, paint)
 
         paint = skia.Paint(
             Style=skia.Paint.kStroke_Style,
             StrokeWidth=5,
             Color=skia.Color(251, 114, 153, 255),
-            AntiAlias=True)
+            AntiAlias=True,
+        )
 
-        image_array = np.bitwise_and(img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                     mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
+        image_array = np.bitwise_and(
+            img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+        )
         canvas = skia.Canvas(image_array, colorType=skia.ColorType.kRGBA_8888_ColorType)
         canvas.drawCircle(radius, radius, radius - 2, paint)
-        return skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                    colorType=skia.ColorType.kRGBA_8888_ColorType).resize(size, size)
+        return skia.Image.fromarray(
+            array=canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            colorType=skia.ColorType.kRGBA_8888_ColorType,
+        ).resize(
+            size, size
+        )  # type: ignore
 
     async def draw_pub_time(self):
         if self.message.pub_ts:
-            pub_time = strftime("%Y-%m-%d %H:%M:%S",
-                                localtime(self.message.pub_ts))
+            pub_time = strftime("%Y-%m-%d %H:%M:%S", localtime(self.message.pub_ts))
         elif self.message.pub_time:
             pub_time = self.message.pub_time
         else:
-            pub_time = strftime("%Y-%m-%d %H:%M:%S", localtime(time()))
+            pub_time = " "
 
-        await DrawText(self.style).draw_text(self.canvas, pub_time, self.style.font.font_size.time,
-                                             (200, 350, 1010, 350, 0,), self.style.color.font_color.sub_title)
+        await DrawText(self.style).draw_text(
+            self.canvas,
+            pub_time,
+            self.style.font.font_size.time,
+            (
+                200,
+                350,
+                1010,
+                350,
+                0,
+            ),
+            self.style.color.font_color.sub_title,
+        )
 
     async def paste_logo(self) -> None:
         logo = skia.Image.open(path.join(self.src_path, "bilibili.png")).resize(231, 105)
         await self.paste(logo, (433, 20))
 
     async def draw_name(self):
         # 如果是大会员的话
@@ -145,40 +162,43 @@
                 color = self.style.color.font_color.name_big_vip
             else:
                 # 到了愚人节大会员名字会变成绿色
                 color = self.style.color.font_color.name_small_vip
         else:
             color = self.style.color.font_color.text
 
-        await DrawText(self.style).draw_text(self.canvas, self.message.name, self.style.font.font_size.name,
-                                             (200, 300, 1010, 300, 0), color)
+        await DrawText(self.style).draw_text(
+            self.canvas,
+            self.message.name,
+            self.style.font.font_size.name,
+            (200, 300, 1010, 300, 0),
+            color,
+        )
 
     async def paste(self, image, position: tuple) -> None:
         x, y = position
         img_height = image.dimensions().fHeight
         img_width = image.dimensions().fWidth
         rec = skia.Rect.MakeXYWH(x, y, img_width, img_height)
-        self.canvas.drawImageRect(image, skia.Rect(
-            0, 0, img_width, img_height), rec)
+        self.canvas.drawImageRect(image, skia.Rect(0, 0, img_width, img_height), rec)
 
 
 class RepostHeader:
     def __init__(self, static_path: str, style: PolyStyle) -> None:
         self.style = style
         self.static_path = static_path
 
     async def run(self, message: Head) -> Optional[np.ndarray]:
-        
         surface = skia.Surface(1080, 100)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*self.style.color.background.repost))
         try:
-            if message.name is None or message.name == "":
+            if not message.name:
                 return None
-            if message.face is not None or message.face=="":
+            if message.face:
                 pos = 140
                 await self.draw_face(message.face, message.mid)
             else:
                 pos = 35
             await self.draw_name(message.name, pos)
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
@@ -186,43 +206,53 @@
             return None
 
     async def draw_face(self, url, mid):
         if url:
             img = await self.get_face(mid, url)
             if img is not None:
                 face = await self.circle_face(img, 80)
-                await paste(self.canvas, face, (40, 10))
+            await paste(self.canvas, face, (40, 10))
 
     async def draw_name(self, name, pos: int):
-        await DrawText(self.style).draw_text(self.canvas, name, self.style.font.font_size.name, (pos, 70, 1010, 70, 0),
-                                             self.style.color.font_color.rich_text)
+        await DrawText(self.style).draw_text(
+            self.canvas,
+            name,
+            self.style.font.font_size.name,
+            (pos, 70, 1010, 70, 0),
+            self.style.color.font_color.rich_text,
+        )
 
     async def circle_face(self, img, size):
-        surface = skia.Surface(img.dimensions().width(),
-                               img.dimensions().height())
+        surface = skia.Surface(img.dimensions().width(), img.dimensions().height())
         mask = surface.getCanvas()
         paint = skia.Paint(
             Style=skia.Paint.kFill_Style,
             Color=skia.Color(255, 255, 255, 255),
-            AntiAlias=True)
+            AntiAlias=True,
+        )
         radius = int(img.dimensions().width() / 2)
         mask.drawCircle(radius, radius, radius, paint)
 
         paint = skia.Paint(
             Style=skia.Paint.kStroke_Style,
             StrokeWidth=5,
             Color=skia.Color(251, 114, 153, 255),
-            AntiAlias=True)
+            AntiAlias=True,
+        )
 
-        image_array = np.bitwise_and(img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                     mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
+        image_array = np.bitwise_and(
+            img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+        )
         canvas = skia.Canvas(image_array, colorType=skia.ColorType.kRGBA_8888_ColorType)
         canvas.drawCircle(radius, radius, radius - 2, paint)
-        return skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                    colorType=skia.ColorType.kRGBA_8888_ColorType).resize(size, size)
+        return skia.Image.fromarray(
+            canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            colorType=skia.ColorType.kRGBA_8888_ColorType,
+        ).resize(size, size)
 
     async def get_face(self, mid, url):
         img_name = f"{mid}.webp"
         img_url = f"{url}@240w_240h_1c_1s.webp"
         img_path = path.join(self.static_path, "Cache", "Face", img_name)
         if path.exists(img_path):
             if time() - int(path.getmtime(img_path)) <= 43200:
@@ -240,30 +270,34 @@
         self.canvas = None
 
     async def run(self) -> Optional[np.ndarray]:
         surface = skia.Surface(1080, 110)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*self.style.color.background.normal))
         try:
-
             now = strftime("%Y-%m-%d %H:%M:%S", localtime(time()))
             render_time = f"图片生成于：{now}"
 
-            await DrawText(self.style).draw_text(self.canvas, render_time, self.style.font.font_size.title,
-                                                 (35, 70, 1010, 70, 0), self.style.color.font_color.sub_title)
+            await DrawText(self.style).draw_text(
+                self.canvas,
+                render_time,
+                self.style.font.font_size.title,
+                (35, 70, 1010, 70, 0),
+                self.style.color.font_color.sub_title,
+            )
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
     async def draw_shadow(self, canvas, pos: tuple, corner: int, bg_color):
         x, y, width, height = pos
         rec = skia.Rect.MakeXYWH(x, y, width, height)
         paint = skia.Paint(
             Color=skia.Color(*bg_color),
             AntiAlias=True,
-            ImageFilter=skia.ImageFilters.DropShadow(0, 0, 10, 10, skia.Color(120, 120, 120))
+            ImageFilter=skia.ImageFilters.DropShadow(0, 0, 10, 10, skia.Color(120, 120, 120)),
         )
         if corner != 0:
             canvas.drawRoundRect(rec, corner, corner, paint)
         else:
             canvas.drawRect(rec, paint)
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynMajor.py` & `dynrender_skia-0.2.6/dynrender_skia/DynMajor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,68 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 @File    :   DynMajor.py
-@Time    :   2023/07/16 20:21:46
+@Time    :   2023/11/13 19:15:46
 @Author  :   Polyisoprene
 @Version :   1.0
 @Desc    :   None
-'''
+"""
+
+from abc import ABC, abstractmethod
+from math import ceil
 from os import path
+from typing import Optional
 
-import skia
-import numpy as np
 import emoji
-from typing import Optional
+import numpy as np
+import skia
+from dynamicadaptor.Content import RichTextDetail
+from dynamicadaptor.Content import Text
+from dynamicadaptor.Majors import Major, RichTextNodes
 from loguru import logger
+
 from .DynStyle import PolyStyle
-from .DynTools import paste, get_pictures, merge_pictures
-from dynamicadaptor.Majors import Major
-from dynamicadaptor.Content import Text
-from math import ceil
 from .DynText import BiliText
-from os import path
-from abc import ABC, abstractmethod
+from .DynTools import paste, get_pictures, merge_pictures
+
 
 class AbstractMajor(ABC):
-    def __init__(self, src_path: str, style: PolyStyle, dyn_major: Major=None) -> None:
+    def __init__(self, src_path: str, style: PolyStyle, dyn_major: Major = None) -> None:
         self.style = style
         self.major = dyn_major
-        self.text_font = skia.Font(skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
-                                   self.style.font.font_size.text)
+        self.text_font = skia.Font(
+            skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
+            self.style.font.font_size.text,
+        )
         self.emoji_font = skia.Font(
             skia.Typeface.MakeFromName(self.style.font.emoji_font_family, self.style.font.font_style),
-            self.style.font.font_size.text)
+            self.style.font.font_size.text,
+        )
         self.src_path = src_path
         self.canvas = None
 
     @abstractmethod
     async def run(self, repost) -> Optional[np.ndarray]:
         pass
 
-    async def draw_text(self, canvas, text: str, font_size, pos: tuple, font_color: tuple,font_style = None):
+    async def draw_text(
+        self,
+        canvas,
+        text: str,
+        font_size,
+        pos: tuple,
+        font_color: tuple,
+        font_style=None,
+    ):
         paint = skia.Paint(AntiAlias=True, Color=skia.Color(*font_color))
         if font_style is not None:
-            self.text_font = skia.Font(skia.Typeface.MakeFromName(self.style.font.font_family, font_style),
-                                   self.style.font.font_size.text)
-        self.text_font.setSize(font_size)
+            self.text_font = skia.Font(
+                skia.Typeface.MakeFromName(self.style.font.font_family, font_style),
+                self.style.font.font_size.text,
+            )
+        self.text_font.setSize(font_size)  # todo:repitition in DynMajor.py line 88
         self.emoji_font.setSize(font_size)
         text = text.replace("\t", "")
         emoji_info = await self.get_emoji_text(text)
         total = len(text) - 1
         x, y, x_bound, y_bound, y_int = pos
         offset = 0
         while offset <= total:
@@ -59,18 +74,18 @@
                 offset = emoji_info[offset][0]
                 font = self.emoji_font
             else:
                 offset += 1
                 font = self.text_font
             if font.textToGlyphs(j)[0] == 0:
                 if typeface := skia.FontMgr().matchFamilyStyleCharacter(
-                        self.style.font.font_family,
-                        self.style.font.font_style,
-                        ["zh", "en"],
-                        ord(j[0]),
+                    self.style.font.font_family,
+                    self.style.font.font_style,
+                    ["zh", "en"],
+                    ord(j[0]),
                 ):
                     font = skia.Font(typeface, font_size)
                 else:
                     font = self.text_font
             measure = font.measureText(j)
             blob = skia.TextBlob(j, font)
             canvas.drawTextBlob(blob, x, y, paint)
@@ -92,72 +107,79 @@
 
     async def draw_shadow(self, canvas, pos: tuple, corner: int, bg_color):
         x, y, width, height = pos
         rec = skia.Rect.MakeXYWH(x, y, width, height)
         paint = skia.Paint(
             Color=skia.Color(*bg_color),
             AntiAlias=True,
-            ImageFilter=skia.ImageFilters.DropShadow(0, 0, 10, 10, skia.Color(120, 120, 120))
+            ImageFilter=skia.ImageFilters.DropShadow(0, 0, 10, 10, skia.Color(120, 120, 120)),
         )
         if corner != 0:
             canvas.drawRoundRect(rec, corner, corner, paint)
         else:
             canvas.drawRect(rec, paint)
 
     async def make_round_cornor(self, img, corner: int):
         surface = skia.Surface(img.width(), img.height())
         mask = surface.getCanvas()
         paint = skia.Paint(
             Style=skia.Paint.kFill_Style,
             Color=skia.Color(255, 255, 255, 255),
-            AntiAlias=True)
+            AntiAlias=True,
+        )
         rect = skia.Rect.MakeXYWH(0, 0, img.width(), img.height())
         mask.drawRoundRect(rect, corner, corner, paint)
-        image_array = np.bitwise_and(img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                     mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
+        image_array = np.bitwise_and(
+            img.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            mask.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+        )
         return skia.Image.fromarray(image_array, colorType=skia.ColorType.kRGBA_8888_ColorType)
 
     async def make_tag(self, tag: str, font_size: int):
         self.text_font.setSize(font_size)
         size = self.text_font.measureText(tag)
         surface = skia.Surface(int(size + 20), int(self.text_font.getSize() + 20))
         canvas = surface.getCanvas()
         canvas.clear(skia.Color(*self.style.color.font_color.name_big_vip))
         blob = skia.TextBlob(tag, self.text_font)
         paint = skia.Paint(AntiAlias=True, Color=skia.Color4f.kWhite)
         canvas.drawTextBlob(blob, 10, int(self.text_font.getSize() + 5), paint)
-        tag_img = skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                       colorType=skia.ColorType.kRGBA_8888_ColorType)
+        tag_img = skia.Image.fromarray(
+            canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            colorType=skia.ColorType.kRGBA_8888_ColorType,
+        )
         tag_img = await self.make_round_cornor(tag_img, 10)
         await paste(self.canvas, tag_img, (1010 - tag_img.width(), 50))
 
     async def make_sub_tag(self, sub_tag: str, font_size: int):
         self.text_font.setSize(font_size)
         size = self.text_font.measureText(sub_tag)
         surface = skia.Surface(int(size + 20), int(self.text_font.getSize() + 20))
         canvas = surface.getCanvas()
         canvas.clear(skia.Color(0, 0, 0, 150))
         blob = skia.TextBlob(sub_tag, self.text_font)
         paint = skia.Paint(AntiAlias=True, Color=skia.Color4f.kWhite)
         canvas.drawTextBlob(blob, 10, int(self.text_font.getSize() + 5), paint)
-        sub_title_img = skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                             colorType=skia.ColorType.kRGBA_8888_ColorType)
+        sub_title_img = skia.Image.fromarray(
+            canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+            colorType=skia.ColorType.kRGBA_8888_ColorType,
+        )
         await paste(self.canvas, await self.make_round_cornor(sub_title_img, 10), (80, 525))
 
 
 class BiliMajor:
     def __init__(self, static_path: str, style: PolyStyle) -> None:
         self.src_path = path.join(static_path, "Src")
         self.style = style
 
     async def run(self, dyn_major: Major, repost: bool = False) -> Optional[np.ndarray]:
         try:
             major_type = dyn_major.type
             if major_type == "MAJOR_TYPE_DRAW":
-                return await DynMajorDraw(self.style,items=dyn_major.draw.items).run(repost)
+                return await DynMajorDraw(self.style, items=dyn_major.draw.items).run(repost)
             elif major_type == "MAJOR_TYPE_ARCHIVE":
                 return await DynMajorArchive(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_LIVE_RCMD":
                 return await DynMajorLiveRcmd(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_OPUS":
                 return await DynMajorOpus(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_ARTICLE":
@@ -175,26 +197,25 @@
             elif major_type == "MAJOR_TYPE_UGC_SEASON":
                 return await DynMajorUgc(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_LIVE":
                 return await DynMajorLive(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_NONE":
                 return await DynMajorNone(self.src_path, self.style, dyn_major).run(repost)
             elif major_type == "MAJOR_TYPE_BLOCKED":
-
                 return await DynMajorBlocked(self.src_path, self.style, dyn_major).run(repost)
             else:
                 logger.warning(f"{major_type} is not supported")
                 return None
         except Exception as e:
             logger.exception(e)
             return None
 
 
-class DynMajorDraw():
-    def __init__(self,style: PolyStyle,items=None) -> None:
+class DynMajorDraw:
+    def __init__(self, style: PolyStyle, items=None) -> None:
         self.style = style
         self.items = items
 
     async def run(self, repost: bool) -> Optional[np.ndarray]:
         """
         make image of major draw
         @param repost: bool
@@ -283,105 +304,144 @@
             if x > 1000:
                 x = 11
                 y += 356
         return canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
 
 
 class DynMajorArchive(AbstractMajor):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         tv = skia.Image.open(path.join(self.src_path, "tv.png")).resize(130, 130)
         try:
             cover = await get_pictures(f"{self.major.archive.cover}@505w_285h_1c.webp", (1010, 570))
 
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await self.draw_text(self.canvas, self.major.archive.title, self.style.font.font_size.text,
-                                 (60, 650, 980, 600, 10), self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.archive.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
             await paste(self.canvas, tv, (905, 455))
-            if self.major.archive.badge is not None and self.major.archive.badge.text != '':
+            if self.major.archive.badge is not None and self.major.archive.badge.text != "":
                 await self.make_tag(self.major.archive.badge.text, self.style.font.font_size.text)
             await self.make_sub_tag(self.major.archive.duration_text, self.style.font.font_size.title)
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception:
             logger.exception("Error")
             return None
 
 
 class DynMajorLiveRcmd(AbstractMajor):
-
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
-            cover = await get_pictures(f"{self.major.live_rcmd.content.live_play_info.cover}@505w_285h_1c.webp",
-                                       (1010, 570))
+            cover = await get_pictures(
+                f"{self.major.live_rcmd.content.live_play_info.cover}@505w_285h_1c.webp",
+                (1010, 570),
+            )
 
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
 
-            await self.draw_text(self.canvas, self.major.live_rcmd.content.live_play_info.title,
-                                 self.style.font.font_size.text, (60, 650, 980, 600, 10),
-                                 self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.live_rcmd.content.live_play_info.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
             await self.make_tag("直播中", self.style.font.font_size.text)
-            await self.make_sub_tag(self.major.live_rcmd.content.live_play_info.watched_show.text_large,
-                                    self.style.font.font_size.title)
+            await self.make_sub_tag(
+                self.major.live_rcmd.content.live_play_info.watched_show.text_large,
+                self.style.font.font_size.title,
+            )
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception:
             logger.exception("Error")
             return None
 
 
 class DynMajorOpus(AbstractMajor):
+    @staticmethod
+    def _convert_to_rich_text_detail(rich_text_node: RichTextNodes) -> RichTextDetail:
+        """
+        Magic method to convert rich_text_node to RichTextDetail.
+        Simplifies the process by directly integrating condition into assignment.
+        :param rich_text_node: RichTextNodes
+        :return: RichTextDetail
+        """
+        return RichTextDetail(
+            type=rich_text_node.type,
+            text=rich_text_node.text,
+            orig_text=rich_text_node.orig_text,
+            emoji=rich_text_node.emoji.dict() if rich_text_node.type == "RICH_TEXT_NODE_TYPE_EMOJI" else None,
+        )
 
     async def run(self, repost) -> Optional[np.ndarray]:
         pics = []
         try:
             if self.major.opus.title:
-               title = await self.make_title(self.major.opus.title,repost)
-               pics.append(title)
+                title = await self.make_title(self.major.opus.title, repost)
+                pics.append(title)
         except Exception as e:
             logger.exception(e)
         try:
             if self.major.opus.summary:
-                dyn_text = Text(text=self.major.opus.summary.text,topic=None,rich_text_nodes=self.major.opus.summary.rich_text_nodes)
-                text_img = await BiliText(path.dirname(self.src_path),self.style).run(dyn_text,repost)
+                # self.style.font.font_style=skia.FontStyle().Normal()
+                dyn_text = Text(
+                    text=self.major.opus.summary.text,
+                    topic=None,
+                    rich_text_nodes=[
+                        self._convert_to_rich_text_detail(node) for node in self.major.opus.summary.rich_text_nodes
+                    ],
+                )
+                text_img = await BiliText(path.dirname(self.src_path), self.style).run(dyn_text, repost)
                 pics.append(text_img)
         except Exception as e:
             logger.exception(e)
         try:
             if self.major.opus.pics:
-                cover =  await DynMajorDraw(self.style,items=self.major.opus.pics).run(repost)
+                cover = await DynMajorDraw(self.style, items=self.major.opus.pics).run(repost)
                 pics.append(cover)
         except Exception as e:
             logger.exception(e)
         if not pics:
             return None
         return await merge_pictures(pics)
 
-    async def make_title(self,title,repost):
+    async def make_title(self, title, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
-        surface = skia.Surface(1080, self.style.font.font_size.name+20)
+        surface = skia.Surface(1080, self.style.font.font_size.name + 20)
         canvas = surface.getCanvas()
         canvas.clear(skia.Color(*background_color))
-        await self.draw_text(canvas,title,self.style.font.font_size.name,(45,int((self.style.font.font_size.name+40)/2),1035,40,0),self.style.color.font_color.text,skia.FontStyle().Bold())
+        await self.draw_text(
+            canvas,
+            title,
+            self.style.font.font_size.name,
+            (45, int((self.style.font.font_size.name + 40) / 2), 1035, 40, 0),
+            self.style.color.font_color.text,
+            font_style=skia.FontStyle().Bold(),
+        )
         return canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
 
-class DynMajorArticle(AbstractMajor):
 
+class DynMajorArticle(AbstractMajor):
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 640)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.draw_shadow(self.canvas, (35, 20, 1010, 600), 20, background_color)
@@ -404,23 +464,38 @@
         else:
             img = await get_pictures(f"{self.major.article.covers[0]}@647w_150h_1c.webp", (1010, 300))
             await paste(self.canvas, img, (35, 20))
 
     async def draw_title_and_desc(self):
         title = self.major.article.title
         if len(self.major.article.covers) > 1:
-            await self.draw_text(self.canvas, title, self.style.font.font_size.text, (50, 410, 960, 330, 0),
-                                 self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                title,
+                self.style.font.font_size.text,
+                (50, 410, 960, 330, 0),
+                self.style.color.font_color.text,
+            )
         else:
-            await self.draw_text(self.canvas, title, self.style.font.font_size.text, (50, 390, 960, 330, 0),
-                                 self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                title,
+                self.style.font.font_size.text,
+                (50, 390, 960, 330, 0),
+                self.style.color.font_color.text,
+            )
         desc = self.major.article.desc
-        await self.draw_text(self.canvas, desc, self.style.font.font_size.title,
-                             (65, 460, 980, 620, int(self.style.font.font_size.title * 1.8)),
-                             self.style.color.font_color.sub_title)
+        await self.draw_text(
+            self.canvas,
+            desc,
+            self.style.font.font_size.title,
+            (65, 460, 980, 620, int(self.style.font.font_size.title * 1.8)),
+            self.style.color.font_color.sub_title,
+        )
+
 
 class DynMajorCommon(AbstractMajor):
     async def run(self, repost) -> Optional[np.ndarray]:
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 285)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
@@ -435,34 +510,50 @@
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
     async def make_title(self):
         title = self.major.common.title
-        await self.draw_text(self.canvas, title, self.style.font.font_size.text, (310, 120, 950, 120, 0),
-                             self.style.color.font_color.text)
+        await self.draw_text(
+            self.canvas,
+            title,
+            self.style.font.font_size.text,
+            (310, 120, 950, 120, 0),
+            self.style.color.font_color.text,
+        )
         sub_title = self.major.common.desc
-        await  self.draw_text(self.canvas, sub_title, self.style.font.font_size.title, (310, 190, 970, 190, 0),
-                              self.style.color.font_color.sub_title)
+        await self.draw_text(
+            self.canvas,
+            sub_title,
+            self.style.font.font_size.title,
+            (310, 190, 970, 190, 0),
+            self.style.color.font_color.sub_title,
+        )
 
     async def make_common_tag(self):
         if self.major.common.badge is not None and self.major.common.badge.text != "":
             self.text_font.setSize(self.style.font.font_size.sub_title)
             size = self.text_font.measureText(self.major.common.badge.text)
             tag_width = int(size + 20)
             surface = skia.Surface(tag_width, int(self.text_font.getSize() + 20))
             canvas = surface.getCanvas()
             canvas.clear(skia.Color(*self.style.color.font_color.name_big_vip))
             blob = skia.TextBlob(self.major.common.badge.text, self.text_font)
             paint = skia.Paint(AntiAlias=True, Color=skia.Color4f.kWhite)
             canvas.drawTextBlob(blob, 10, int(self.text_font.getSize() + 5), paint)
-            tag_img = skia.Image.fromarray(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
-                                           colorType=skia.ColorType.kRGBA_8888_ColorType)
-            await paste(self.canvas, await self.make_round_cornor(tag_img, 10), (280 - tag_width - 20, 40))
+            tag_img = skia.Image.fromarray(
+                canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType),
+                colorType=skia.ColorType.kRGBA_8888_ColorType,
+            )
+            await paste(
+                self.canvas,
+                await self.make_round_cornor(tag_img, 10),
+                (280 - tag_width - 20, 40),
+            )
 
 
 class DynMajorMusic(AbstractMajor):
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 285)
         self.canvas = surface.getCanvas()
@@ -477,65 +568,83 @@
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
     async def make_title(self):
         title = self.major.music.title
-        await self.draw_text(self.canvas, title, self.style.font.font_size.text, (310, 120, 950, 120, 0),
-                             self.style.color.font_color.text)
+        await self.draw_text(
+            self.canvas,
+            title,
+            self.style.font.font_size.text,
+            (310, 120, 950, 120, 0),
+            self.style.color.font_color.text,
+        )
         sub_title = self.major.music.label
-        await self.draw_text(self.canvas, sub_title, self.style.font.font_size.title, (310, 190, 970, 190, 0),
-                             self.style.color.font_color.sub_title)
+        await self.draw_text(
+            self.canvas,
+            sub_title,
+            self.style.font.font_size.title,
+            (310, 190, 970, 190, 0),
+            self.style.color.font_color.sub_title,
+        )
 
 
 class DynMajorPgc(AbstractMajor):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         tv = skia.Image.open(path.join(self.src_path, "tv.png")).resize(130, 130)
         try:
             cover = await get_pictures(f"{self.major.pgc.cover}@505w_285h_1c.webp", (1010, 570))
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await self.draw_text(self.canvas, self.major.pgc.title, self.style.font.font_size.text,
-                                 (60, 650, 980, 600, 10), self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.pgc.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
             await paste(self.canvas, tv, (905, 455))
-            if self.major.pgc.badge is not None and self.major.pgc.badge.text != '':
+            if self.major.pgc.badge is not None and self.major.pgc.badge.text != "":
                 tag = self.major.pgc.badge.text
             else:
                 tag = "投稿视频"
             await self.make_tag(tag, self.style.font.font_size.text)
             await self.make_sub_tag(f"{self.major.pgc.stat.play}播放", self.style.font.font_size.title)
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception:
             logger.exception("Error")
             return None
 
 
 class DynMajorMediaList(AbstractMajor):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         tv = skia.Image.open(path.join(self.src_path, "tv.png")).resize(130, 130)
         try:
             cover = await get_pictures(f"{self.major.medialist.cover}@505w_285h_1c.webp", (1010, 570))
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await self.draw_text(self.canvas, self.major.medialist.title, self.style.font.font_size.text,
-                                 (60, 650, 980, 600, 10), self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.medialist.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
             if self.major.medialist.badge is not None:
                 tag = self.major.medialist.badge.text
             else:
                 tag = "投稿视频"
             await self.make_tag(tag, self.style.font.font_size.text)
             await self.make_sub_tag(self.major.medialist.sub_title, self.style.font.font_size.title)
@@ -543,134 +652,167 @@
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
 
 class DynMajorCourses(AbstractMajor):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         tv = skia.Image.open(path.join(self.src_path, "tv.png")).resize(130, 130)
         try:
             cover = await get_pictures(f"{self.major.courses.cover}@505w_285h_1c.webp", (1010, 570))
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await self.draw_text(self.canvas, self.major.courses.title, self.style.font.font_size.text,
-                                 (60, 650, 980, 600, 10), self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.courses.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
-            if self.major.courses.badge is not None and self.major.courses.badge.text != '':
+            if self.major.courses.badge is not None and self.major.courses.badge.text != "":
                 tag = self.major.courses.badge.text
             else:
                 tag = "投稿视频"
             await self.make_tag(tag, self.style.font.font_size.text)
             await self.make_sub_tag(self.major.courses.desc, self.style.font.font_size.title)
             await paste(self.canvas, tv, (905, 455))
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
 
 class DynMajorUgc(AbstractMajor):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         tv = skia.Image.open(path.join(self.src_path, "tv.png")).resize(130, 130)
         try:
             cover = await get_pictures(f"{self.major.ugc_season.cover}@505w_285h_1c.webp", (1010, 570))
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await self.draw_text(self.canvas, self.major.ugc_season.title, self.style.font.font_size.text,
-                                 (60, 650, 980, 600, 10), self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.ugc_season.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
-            if self.major.ugc_season.badge is not None and self.major.ugc_season.badge.text != '':
+            if self.major.ugc_season.badge is not None and self.major.ugc_season.badge.text != "":
                 tag = self.major.ugc_season.badge.text
             else:
                 tag = "投稿视频"
             await self.make_tag(tag, self.style.font.font_size.text)
             await self.make_sub_tag(self.major.ugc_season.duration_text, self.style.font.font_size.title)
             await paste(self.canvas, tv, (905, 455))
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
 
 class DynMajorLive(AbstractMajor):
-
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 695)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             cover = await get_pictures(f"{self.major.live.cover}@505w_285h_1c.webp", (1010, 570))
             await self.draw_shadow(self.canvas, (35, 25, 1010, 655), 20, background_color)
             rec = skia.Rect.MakeXYWH(35, 25, 1010, 665)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await self.draw_text(self.canvas, self.major.live.title, self.style.font.font_size.text,
-                                 (60, 650, 980, 600, 10), self.style.color.font_color.text)
+            await self.draw_text(
+                self.canvas,
+                self.major.live.title,
+                self.style.font.font_size.text,
+                (60, 650, 980, 600, 10),
+                self.style.color.font_color.text,
+            )
             await paste(self.canvas, cover, (35, 25))
-            if self.major.live.badge is not None and self.major.live.badge.text != '':
+            if self.major.live.badge is not None and self.major.live.badge.text != "":
                 tag = self.major.live.badge.text
             else:
                 tag = "投稿视频"
             await self.make_tag(tag, self.style.font.font_size.text)
 
             await self.make_sub_tag(self.major.live.desc_second, self.style.font.font_size.title)
 
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
 
 
 class DynMajorNone(AbstractMajor):
-    
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 100)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
             await self.make_tips()
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
             return None
-        
+
     async def make_tips(self):
         error = skia.Image.open(path.join(self.src_path, "error.png")).resize(40, 40)
-        await self.draw_text(self.canvas,self.major.none.tips,self.style.font.font_size.text,(90,60,1080,40,0),self.style.color.font_color.sub_title)
+        await self.draw_text(
+            self.canvas,
+            self.major.none.tips,
+            self.style.font.font_size.text,
+            (90, 60, 1080, 40, 0),
+            self.style.color.font_color.sub_title,
+        )
         await paste(self.canvas, error, (40, 30))
 
+
 class DynMajorBlocked(AbstractMajor):
     async def run(self, repost):
         background_color = self.style.color.background.repost if repost else self.style.color.background.normal
         surface = skia.Surface(1080, 1200)
         self.canvas = surface.getCanvas()
         self.canvas.clear(skia.Color(*background_color))
         try:
-            result = await get_pictures([f"{self.major.blocked.bg_img.img_dark}@1c.webp",self.major.blocked.icon.img_day])            
+            result = await get_pictures(
+                [
+                    f"{self.major.blocked.bg_img.img_dark}@1c.webp",
+                    self.major.blocked.icon.img_day,
+                ]
+            )
             await self.draw_shadow(self.canvas, (40, 100, 1000, 1000), 20, background_color)
             rec = skia.Rect.MakeXYWH(40, 100, 1000, 1000)
             self.canvas.clipRRect(skia.RRect(rec, 20, 20), skia.ClipOp.kIntersect)
-            await paste(self.canvas,result[1],(456,380))
-            await paste(self.canvas, result[0].resize(1000,1000), (40, 100))
+            await paste(self.canvas, result[1], (456, 380))
+            await paste(self.canvas, result[0].resize(1000, 1000), (40, 100))
             text = self.major.blocked.hint_message.split("\n")
-            await self.draw_text(self.canvas, text[0], self.style.font.font_size.name,
-                                 (380, 630, 980, 600, 10), self.style.color.font_color.sub_title)
-            await self.draw_text(self.canvas, text[1], self.style.font.font_size.name,
-                                 (160, 700, 980, 600, 10), self.style.color.font_color.sub_title)
+            await self.draw_text(
+                self.canvas,
+                text[0],
+                self.style.font.font_size.name,
+                (380, 630, 980, 600, 10),
+                self.style.color.font_color.sub_title,
+            )
+            await self.draw_text(
+                self.canvas,
+                text[1],
+                self.style.font.font_size.name,
+                (160, 700, 980, 600, 10),
+                self.style.color.font_color.sub_title,
+            )
             return self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
         except Exception as e:
             logger.exception(e)
-            return None
+            return None
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynRepost.py` & `dynrender_skia-0.2.6/dynrender_skia/DynRepost.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 @File    :   DynRepost.py
 @Time    :   2023/07/19 15:33:23
-@Author  :   Polyisoprene 
+@Author  :   Polyisoprene
 @Version :   1.0
 @Desc    :   None
-'''
+"""
+
 import asyncio
 
 from dynamicadaptor.Repost import Forward
 
 from .DynAdditional import BiliAdditional
 from .DynHeader import RepostHeader
 from .DynMajor import BiliMajor
@@ -26,11 +26,10 @@
     async def run(self, message: Forward):
         tasks = [RepostHeader(self.static_path, self.style).run(message.header)]
         if message.text is not None:
             tasks.append(BiliText(self.static_path, self.style).run(message.text, repost=True))
         if message.major is not None:
             tasks.append(BiliMajor(self.static_path, self.style).run(message.major, True))
         if message.additional is not None:
-            
             tasks.append(BiliAdditional(self.static_path, self.style).run(message.additional, True))
         result = await asyncio.gather(*tasks)
-        return await merge_pictures(result)
+        return await merge_pictures(result) # type: ignore
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynStyle.py` & `dynrender_skia-0.2.6/dynrender_skia/DynStyle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 @File    :   DynStyle.py
 @Time    :   2023/07/16 20:42:46
 @Author  :   Polyisoprene
 @Version :   1.0
 @Desc    :   None
-'''
+"""
 
 from typing import Any
 
 from pydantic import BaseModel
 
 
 class FontSize(BaseModel):
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynText.py` & `dynrender_skia-0.2.6/dynrender_skia/DynText.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # @Time    : 2023/7/15 下午8:12
 # @Author  : Polyisoprene
 # @File    : DynText.py
 
 import asyncio
 from os import path
 from typing import Optional
@@ -10,15 +9,15 @@
 import emoji
 import numpy as np
 import skia
 from dynamicadaptor.Content import Text
 from loguru import logger
 
 from .DynStyle import PolyStyle
-from .DynTools import paste, merge_pictures, get_pictures
+from .DynTools import paste, merge_pictures, get_pictures, DrawText
 
 
 class BiliText:
     """渲染动态的文字部分"""
 
     def __init__(self, static_path: str, style: PolyStyle) -> None:
         self.emoji_path = path.join(static_path, "Cache", "Emoji")
@@ -29,27 +28,33 @@
         self.bg_color = None
         self.offset = 40
         self.x_bound = 1030
         self.image_list = []
         self.emoji_dict = {}
 
     async def run(self, dyn_text: Text, repost: bool = False) -> Optional[np.ndarray]:
-        self.text_font = skia.Font(skia.Typeface.MakeFromName(self.style.font.font_family,self.style.font.font_style),self.style.font.font_size.text)
-        self.emoji_font = skia.Font(skia.Typeface.MakeFromName(self.style.font.emoji_font_family,self.style.font.font_style),self.style.font.font_size.text)
+        self.text_font = skia.Font(
+            skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
+            self.style.font.font_size.text,
+        )
+        self.emoji_font = skia.Font(
+            skia.Typeface.MakeFromName(self.style.font.emoji_font_family, self.style.font.font_style),
+            self.style.font.font_size.text,
+        )
         self.bg_color = self.style.color.background.repost if repost else self.style.color.background.normal
         self.canvas.clear(skia.Color(*self.bg_color))
         try:
             tasks = []
             if dyn_text.topic is not None:
                 tasks.append(self.make_topic(dyn_text.topic.name))
             if dyn_text.text:
                 tasks.append(self.make_text_image(dyn_text))
             await asyncio.gather(*tasks)
             return await merge_pictures(self.image_list)
-        except Exception as e:
+        except Exception:
             logger.exception("Error")
             return None
 
     async def make_text_image(self, dyn_text):
         emoji_list = []
         emoji_name_list = []
         rich_list = []
@@ -57,15 +62,15 @@
             if i.type == "RICH_TEXT_NODE_TYPE_EMOJI":
                 if i.text not in emoji_name_list:
                     emoji_name_list.append(i.text)
                     emoji_list.append(i.emoji.icon_url)
             elif i.type != "RICH_TEXT_NODE_TYPE_TEXT":
                 rich_list.append(i)
         result = await asyncio.gather(self.get_emoji(emoji_list, emoji_name_list), self.get_rich_pic(rich_list))
-        await self.draw_text(result[1], dyn_text)
+        await self.draw_text(result[1], dyn_text) # type: ignore
         if self.offset != 40:
             self.image_list.append(self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
 
     async def get_emoji(self, emoji_url: list, emoji_name: list):
         emoji_pic = []
         emoji_index = []
         emoji_url_list = []
@@ -141,54 +146,45 @@
         topic_size = self.style.font.font_size.text
         topic_img = skia.Image.open(path.join(self.src_path, "new_topic.png")).resize(topic_size, topic_size)
         icon_size = int(topic_size * 1.5)
         surface = skia.Surface(1080, icon_size + 10)
         canvas = surface.getCanvas()
         canvas.clear(skia.Color(*self.bg_color))
         await paste(canvas, topic_img, (45, 15))
-
-        paint = skia.Paint(AntiAlias=True, Color=skia.Color(*self.style.color.font_color.rich_text))
-        font_name = None
-        offset = 45 + topic_size + 10
-        font = None
-        for i in topic:
-            if typeface := skia.FontMgr().matchFamilyStyleCharacter(
-                    self.style.font.font_family,
-                    self.style.font.font_style,
-                    ["zh", "en"],
-                    ord(i),
-            ):
-                text_family_name = typeface.getFamilyName()
-                if font_name != text_family_name:
-                    font_name = text_family_name
-                    font = skia.Font(typeface, topic_size)
-            else:
-                font = skia.Font(None, topic_size)
-            blob = skia.TextBlob(i, font)
-            canvas.drawTextBlob(blob, offset, 50, paint)
-            offset += font.measureText(i)
+        await DrawText(self.style).draw_text(
+            canvas,
+            topic,
+            topic_size,
+            (45 + topic_size + 10, 50, 1080, 50, 0),
+            self.style.color.font_color.rich_text,
+        )
         self.image_list.append(canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
 
     async def draw_text(self, rich_list: list, dyn_text: Text):
         self.canvas.clear(skia.Color(*self.bg_color))
-        for i in dyn_text.rich_text_nodes:
-            if i.type in {"RICH_TEXT_NODE_TYPE_AT", "RICH_TEXT_NODE_TYPE_TEXT", "RICH_TEXT_NODE_TYPE_TOPIC"}:
+        for i in dyn_text.rich_text_nodes: # type: ignore
+            if i.type in {
+                "RICH_TEXT_NODE_TYPE_AT",
+                "RICH_TEXT_NODE_TYPE_TEXT",
+                "RICH_TEXT_NODE_TYPE_TOPIC",
+            }:
                 if i.type in {"RICH_TEXT_NODE_TYPE_AT", "RICH_TEXT_NODE_TYPE_TOPIC"}:
                     color = skia.Color(*self.style.color.font_color.rich_text)
                 else:
                     color = skia.Color(*self.style.color.font_color.text)
                 await self.draw_plain_text(i.text, color)
             elif i.type == "RICH_TEXT_NODE_TYPE_EMOJI":
                 await self.draw_emoji(i.text)
             else:
                 await self.draw_rich_text(i, rich_list)
 
     async def draw_plain_text(self, dyn_detail, color):
         font = None
-        dyn_detail = dyn_detail.translate(str.maketrans({'\r': ''}))
+        e=False
+        dyn_detail = dyn_detail.translate(str.maketrans({"\r": ""}))
         paint = skia.Paint(AntiAlias=True, Color=color)
         emoji_info = await self.get_emoji_text(dyn_detail)
         total = len(dyn_detail) - 1
         offset = 0
         while offset <= total:
             j = dyn_detail[offset]
             if j == "\n":
@@ -199,44 +195,51 @@
                 offset += 1
                 self.offset = 40
                 continue
             if offset in emoji_info.keys():
                 j = emoji_info[offset][1]
                 offset = emoji_info[offset][0]
                 font = self.emoji_font
+                e=True
             else:
-                offset +=1
+                offset += 1
                 font = self.text_font
+                e=False
             if font.textToGlyphs(j)[0] == 0:
                 if typeface := skia.FontMgr().matchFamilyStyleCharacter(
                     self.style.font.font_family,
                     self.style.font.font_style,
                     ["zh", "en"],
                     ord(j[0]),
                 ):
                     font = skia.Font(typeface, self.style.font.font_size.text)
                 else:
                     font = self.text_font
-            measure = font.measureText(j)
-            blob = skia.TextBlob(j, font)
-            self.canvas.drawTextBlob(blob, self.offset, 50, paint)
+            if not e:
+                measure = font.measureText(j)
+                blob = skia.TextBlob(j, font)
+                self.canvas.drawTextBlob(blob, self.offset, 50, paint)
+            else:
+                measure = font.measureText(j[0])
+                blob = skia.TextBlob.MakeFromShapedText(j, font)
+                self.canvas.drawTextBlob(blob, self.offset, 5, paint)
             self.offset += measure
             if self.offset > self.x_bound:
                 self.offset = 40
                 self.canvas.saveLayer()
                 self.canvas.clear(skia.Color(*self.bg_color))
                 self.image_list.append(self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
                 self.canvas.restore()
 
-    async def draw_emoji(self,emoji_detail):
+    async def draw_emoji(self, emoji_detail):
         img = self.emoji_dict[emoji_detail]
         if img is not None:
             img_size = img.dimensions().width()
-            await paste(self.canvas,img, (int(self.offset),0))
-            self.offset += img_size+5
+            await paste(self.canvas, img, (int(self.offset), 0))
+            self.offset += img_size + 5
             if self.offset >= self.x_bound:
                 self.canvas.saveLayer()
                 self.canvas.clear(skia.Color(*self.bg_color))
                 self.image_list.append(self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
                 self.canvas.restore()
                 self.offset = 40
 
@@ -247,40 +250,41 @@
             icon = rich_list["lottery"]
         elif text_detail.type == "RICH_TEXT_NODE_TYPE_GOODS":
             icon = rich_list["goods"]
         elif text_detail.type == "RICH_TEXT_NODE_TYPE_CV":
             icon = rich_list["cv"]
         else:
             icon = rich_list["link"]
-        await paste(self.canvas,icon,(int(self.offset),int(60-icon.dimensions().height())/2))
-        self.offset += icon.dimensions().width()+5
+        await paste(
+            self.canvas,
+            icon,
+            (int(self.offset), int(60 - icon.dimensions().height()) / 2),
+        )
+        self.offset += icon.dimensions().width() + 5
         if self.offset >= self.x_bound:
             self.canvas.saveLayer()
             self.canvas.clear(skia.Color(*self.bg_color))
             self.image_list.append(self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
             self.canvas.restore()
             self.offset = 40
         paint = skia.Paint(AntiAlias=True, Color=skia.Color(*self.style.color.font_color.rich_text))
-        font_name = None
-        font = None
+        font = self.text_font
         for i in text_detail.text:
-            if typeface := skia.FontMgr().matchFamilyStyleCharacter(
+            if font.textToGlyphs(i)[0] == 0:
+                if typeface := skia.FontMgr().matchFamilyStyleCharacter(
                     self.style.font.font_family,
                     self.style.font.font_style,
                     ["zh", "en"],
                     ord(i),
-            ):
-                text_family_name = typeface.getFamilyName()
-                if font_name != text_family_name:
-                    font_name = text_family_name
+                ):
                     font = skia.Font(typeface, self.style.font.font_size.text)
-            else:
-                font = skia.Font(None, self.style.font.font_size.text)
+                else:
+                    font = self.text_font
             blob = skia.TextBlob(i, font)
             self.canvas.drawTextBlob(blob, self.offset, 50, paint)
             self.offset += font.measureText(i)
             if self.offset >= self.x_bound:
                 self.canvas.saveLayer()
                 self.canvas.clear(skia.Color(*self.bg_color))
                 self.image_list.append(self.canvas.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType))
                 self.canvas.restore()
-                self.offset = 40
+                self.offset = 40
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/DynTools.py` & `dynrender_skia-0.2.6/dynrender_skia/DynTools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,73 @@
-# -*- coding: utf-8 -*-
 # @Time    : 2023/7/15 下午9:22
 # @Author  : Polyisoprene
 # @File    : DynTools.py
 import asyncio
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Tuple, Dict
 
 import emoji
 import httpx
 import numpy as np
 import skia
 from loguru import logger
 from numpy import ndarray
 
 from .DynStyle import PolyStyle
 
 
-async def get_pictures(url: Union[str, list], size: Optional[tuple] = None):
+async def get_pictures(
+    url: Union[str, List[str]], size: Optional[Tuple[int, int]] = None
+) -> Union[skia.Image, Tuple[skia.Image, ...]]:
     async with httpx.AsyncClient() as client:
         if isinstance(url, list):
             return await asyncio.gather(*[request_img(client, i, size) for i in url])
         elif isinstance(url, str):
             return await request_img(client, url, size)
 
 
-async def request_img(client, url, size):
+async def request_img(client: httpx.AsyncClient, url: str, size: Optional[Tuple[int, int]]) -> Optional[skia.Image]:
+    """
+    Request image from url and return skia.Image
+
+    Args:
+        client: httpx.AsyncClient
+        url: str
+        size: Optional[Tuple[int, int]]
+
+    Returns:
+        Optional[skia.Image]: skia.Image
+    """
     try:
         resp = await client.get(url)
-        assert resp.status_code == 200
-        img = skia.Image.MakeFromEncoded(resp.content)
-        if size is not None and img is not None:
-            return img.resize(*size)
-        return img
-
-    except:
-        logger.exception("e")
-        return None
+        if resp.status_code != 200:
+            raise httpx.HTTPStatusError(
+                f"Request failed with status code {resp.status_code}", request=resp.request, response=resp
+            )
+        img = skia.Image.MakeFromEncoded(encoded=resp.content)  # type: ignore
+        if img is None:
+            logger.error("Failed to decode image")
+            return None
+        return img.resize(*size) if size is not None else img
+    except (httpx.RequestError, httpx.HTTPStatusError) as e:
+        logger.exception(f"Request or HTTP error occurred: {e}")
+    except Exception as e:
+        logger.exception(f"Unexpected error: {e}")
+    return None
 
 
 async def merge_pictures(img_list: List[ndarray]) -> ndarray:
     img_top = np.zeros([0, 1080, 4], np.uint8)
     if len(img_list) == 1 and img_list[0] is not None:
         return img_list[0]
-    for i in img_list:
-        if i is not None:
-            img_top = np.vstack((img_top, i))
+    for img in img_list:
+        if img is None:
+            continue
+        if img.shape[1] != 1080:
+            raise ValueError("The width of the image must be 1080")
+        img_top = np.vstack((img_top, img))
     return img_top
 
 
 async def paste(src, target, position: tuple) -> None:
     try:
         if target is not None:
             x, y = position
@@ -58,46 +78,49 @@
     except Exception as e:
         logger.exception(e)
 
 
 class DrawText:
     def __init__(self, style: PolyStyle):
         self.style = style
-        self.text_font = skia.Font(skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
-                                   self.style.font.font_size.text)
+        self.text_font = skia.Font(
+            skia.Typeface.MakeFromName(self.style.font.font_family, self.style.font.font_style),
+            self.style.font.font_size.text,
+        )
         self.emoji_font = skia.Font(
             skia.Typeface.MakeFromName(self.style.font.emoji_font_family, self.style.font.font_style),
-            self.style.font.font_size.text)
+            self.style.font.font_size.text,
+        )
 
     async def draw_text(self, canvas, text: str, font_size, pos: tuple, font_color: tuple):
         paint = skia.Paint(AntiAlias=True, Color=skia.Color(*font_color))
         self.text_font.setSize(font_size)
         self.emoji_font.setSize(font_size)
         text = text.replace("\t", "")
         emoji_info = await self.get_emoji_text(text)
         total = len(text) - 1
         x, y, x_bound, y_bound, y_int = pos
-        offset = 0
+        offset:int= 0
         while offset <= total:
             j = text[offset]
             if j == "\n":
                 break
             if offset in emoji_info.keys():
                 j = emoji_info[offset][1]
-                offset = emoji_info[offset][0]
+                offset = emoji_info[offset][0] # type: ignore
                 font = self.emoji_font
             else:
                 offset += 1
                 font = self.text_font
             if font.textToGlyphs(j)[0] == 0:
                 if typeface := skia.FontMgr().matchFamilyStyleCharacter(
-                        self.style.font.font_family,
-                        self.style.font.font_style,
-                        ["zh", "en"],
-                        ord(j[0]),
+                    self.style.font.font_family,
+                    self.style.font.font_style,
+                    ["zh", "en"],
+                    ord(j[0]),
                 ):
                     font = skia.Font(typeface, font_size)
                 else:
                     font = self.text_font
             measure = font.measureText(j)
             blob = skia.TextBlob(j, font)
             canvas.drawTextBlob(blob, x, y, paint)
@@ -106,13 +129,14 @@
                 y += y_int
                 if y >= y_bound:
                     blob = skia.TextBlob("...", font)
                     canvas.drawTextBlob(blob, x, y - y_int, paint)
                     break
                 x = pos[0]
 
-    async def get_emoji_text(self, text):
+    @staticmethod
+    async def get_emoji_text(text: str) -> Dict[int, List[Union[int, str]]]:
         result = emoji.emoji_list(text)
         temp = {}
         for i in result:
             temp[i["match_start"]] = [i["match_end"], i["emoji"]]
         return temp
```

### Comparing `dynrender_skia-0.2.5/dynrender_skia/Static.zip` & `dynrender_skia-0.2.6/dynrender_skia/Static.zip`

 * *Files identical despite different names*

