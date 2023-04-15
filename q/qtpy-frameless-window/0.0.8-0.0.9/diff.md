# Comparing `tmp/QtPy-Frameless-Window-0.0.8.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.8.tar", last modified: Wed Apr 12 15:00:20 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.9.tar", last modified: Sat Apr 15 18:03:34 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.8.tar` & `QtPy-Frameless-Window-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.0.8/LICENSE
--rw-r--r--   0        0        0     1000 2023-04-12 14:59:07.447897 QtPy-Frameless-Window-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.0.8/qt_api/__init__.py
--rw-r--r--   0        0        0     1169 2023-04-12 14:27:18.865226 QtPy-Frameless-Window-0.0.8/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 06:26:37.921076 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     1468 2023-04-12 14:50:14.195223 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0      270 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0      457 2023-04-12 08:04:13.929582 QtPy-Frameless-Window-0.0.8/qtframelesswindow/api_differ/windows.py
--rw-r--r--   0        0        0     4351 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.8/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-12 08:04:14.020784 QtPy-Frameless-Window-0.0.8/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0     4533 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.8/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-12 08:04:14.032673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     5064 2023-04-12 14:27:18.868207 QtPy-Frameless-Window-0.0.8/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-12 12:28:36.521987 QtPy-Frameless-Window-0.0.8/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-12 06:26:37.922905 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0     9302 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     8330 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7816 2023-04-12 08:04:14.041673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-12 12:00:49.607910 QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-12 06:26:37.924905 QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8979 2023-04-12 08:04:14.052662 QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1156 2023-04-12 14:26:31.626229 QtPy-Frameless-Window-0.0.8/README.md
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.0.9/LICENSE
+-rw-r--r--   0        0        0      812 2023-04-15 17:58:32.279110 QtPy-Frameless-Window-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.0.9/qt_api/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-15 17:29:48.930752 QtPy-Frameless-Window-0.0.9/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0     6143 2023-04-15 17:22:48.263396 QtPy-Frameless-Window-0.0.9/qtframelesswindow/buttons.py
+-rw-r--r--   0        0        0     1747 2023-04-15 17:15:46.251860 QtPy-Frameless-Window-0.0.9/qtframelesswindow/manager.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:14:22.678018 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-15 05:44:35.457997 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/close.svg
+-rw-r--r--   0        0        0      300 2023-04-15 05:44:35.526063 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/maximize.svg
+-rw-r--r--   0        0        0      157 2023-04-15 05:44:35.461990 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/minimize.svg
+-rw-r--r--   0        0        0      393 2023-04-15 05:44:35.461002 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/black/normalize.svg
+-rw-r--r--   0        0        0      389 2023-04-15 05:45:07.996660 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/close.svg
+-rw-r--r--   0        0        0      300 2023-04-15 05:45:07.996660 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/maximize.svg
+-rw-r--r--   0        0        0      157 2023-04-15 05:45:08.057658 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/minimize.svg
+-rw-r--r--   0        0        0      393 2023-04-15 05:45:07.987656 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/images/white/normalize.svg
+-rw-r--r--   0        0        0      214 2023-04-15 09:26:53.084385 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/qss/button.qss
+-rw-r--r--   0        0        0      222 2023-04-15 14:57:53.483029 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/qss/button_close.qss
+-rw-r--r--   0        0        0     7069 2023-04-15 17:13:26.713324 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource.py
+-rw-r--r--   0        0        0      479 2023-04-15 17:13:16.687205 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource.qrc
+-rw-r--r--   0        0        0     7072 2023-04-15 18:02:59.241478 QtPy-Frameless-Window-0.0.9/qtframelesswindow/resource/resource_rc.py
+-rw-r--r--   0        0        0     7026 2023-04-15 17:32:36.258010 QtPy-Frameless-Window-0.0.9/qtframelesswindow/window.py
+-rw-r--r--   0        0        0     1578 2023-04-15 18:02:09.368876 QtPy-Frameless-Window-0.0.9/README.md
+-rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.9/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.8/LICENSE` & `QtPy-Frameless-Window-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.9/qtframelesswindow/window.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,258 +1,181 @@
-# coding:utf-8
-import sys
-from ctypes import cast
-from ctypes.wintypes import LPRECT, MSG
-
-import win32api
-import win32con
-import win32gui
-from qtpy.QtCore import Qt
-from qtpy.QtGui import QCloseEvent, QCursor
-from qtpy.QtWidgets import QApplication, QWidget, QMainWindow, QDialog
-
-from ..titlebar import TitleBar
-from ..utils import win32_utils as win_utils
-from ..utils.win32_utils import Taskbar
-from .c_structures import LPNCCALCSIZE_PARAMS
-from .window_effect import WindowsWindowEffect
-
-
-class Ui_Frameless(object):
-    BORDER_WIDTH = 5
-
-    def __init__(self, *args, **kwds) -> None:
-        pass
-
-    def setupUi(self, Form: QWidget):
-        self.windowEffect = WindowsWindowEffect(Form)
-        self.titleBar = TitleBar(Form)
-        self.resize(500, 500)
-        self.titleBar.raise_()
-        self._Form = Form
-        self._isResizeEnabled = True
-
-    def setTitleBar(self, titleBar: QWidget):
-        """set custom title bar
-
-        Parameters
-        ----------
-        titleBar: TitleBar
-            title bar
-        """
-        self.titleBar.deleteLater()
-        self.titleBar = titleBar
-        self.titleBar.setParent(self)
-        self.titleBar.raise_()
-
-    def resizeFrameless(self):
-        self.titleBar.resize(self._Form.width(), self.titleBar.height())
-
-    def nativeFrameless(self, message):
-        """Handle the Windows message"""
-        msg = MSG.from_address(message.__int__())
-        if not msg.hWnd:
-            return False, 0
-
-        if msg.message == win32con.WM_NCHITTEST and self._isResizeEnabled:
-            pos = QCursor.pos()
-            xPos = pos.x() - self._Form.x()
-            yPos = pos.y() - self._Form.y()
-            w, h = self._Form.width(), self._Form.height()
-            lx = xPos < self.BORDER_WIDTH
-            rx = xPos > w - self.BORDER_WIDTH
-            ty = yPos < self.BORDER_WIDTH
-            by = yPos > h - self.BORDER_WIDTH
-            if lx and ty:
-                return True, win32con.HTTOPLEFT
-            elif rx and by:
-                return True, win32con.HTBOTTOMRIGHT
-            elif rx and ty:
-                return True, win32con.HTTOPRIGHT
-            elif lx and by:
-                return True, win32con.HTBOTTOMLEFT
-            elif ty:
-                return True, win32con.HTTOP
-            elif by:
-                return True, win32con.HTBOTTOM
-            elif lx:
-                return True, win32con.HTLEFT
-            elif rx:
-                return True, win32con.HTRIGHT
-        elif msg.message == win32con.WM_NCCALCSIZE:
-            if msg.wParam:
-                rect = cast(msg.lParam, LPNCCALCSIZE_PARAMS).contents.rgrc[0]
-            else:
-                rect = cast(msg.lParam, LPRECT).contents
+from qtpy.QtCore import Qt, QCoreApplication, QEvent, QPropertyAnimation, QRect
+from qtpy.QtGui import QPaintEvent, QPainter, QColor
+from qtpy.QtWidgets import QWidget, QVBoxLayout, QMainWindow, QDialog
+from .buttons import TitleBar
+from .manager import Theme
+import math
 
-            isMax = win_utils.isMaximized(msg.hWnd)
-            isFull = win_utils.isFullScreen(msg.hWnd)
 
-            # adjust the size of client rect
-            if isMax and not isFull:
-                ty = win_utils.getResizeBorderThickness(msg.hWnd, False)
-                rect.top += ty
-                rect.bottom -= ty
-
-                tx = win_utils.getResizeBorderThickness(msg.hWnd, True)
-                rect.left += tx
-                rect.right -= tx
-
-            # handle the situation that an auto-hide taskbar is enabled
-            if (isMax or isFull) and Taskbar.isAutoHide():
-                position = Taskbar.getPosition(msg.hWnd)
-                if position == Taskbar.LEFT:
-                    rect.top += Taskbar.AUTO_HIDE_THICKNESS
-                elif position == Taskbar.BOTTOM:
-                    rect.bottom -= Taskbar.AUTO_HIDE_THICKNESS
-                elif position == Taskbar.LEFT:
-                    rect.left += Taskbar.AUTO_HIDE_THICKNESS
-                elif position == Taskbar.RIGHT:
-                    rect.right -= Taskbar.AUTO_HIDE_THICKNESS
-
-            result = 0 if not msg.wParam else win32con.WVR_REDRAW
-            return True, result
-
-        return False, 0
-
-    def setResizeEnabled(self, isEnabled: bool):
-        """set whether resizing is enabled"""
-        self._isResizeEnabled = isEnabled
-
-    def setScreenChanged(self):
-        # solve issue #5
-        self._Form.windowHandle().screenChanged.connect(self.__onScreenChanged)
-
-    def __onScreenChanged(self):
-        hWnd = int(self._Form.windowHandle().winId())
-        win32gui.SetWindowPos(
-            hWnd,
-            None,
-            0,
-            0,
-            0,
-            0,
-            win32con.SWP_NOMOVE | win32con.SWP_NOSIZE | win32con.SWP_FRAMECHANGED,
-        )
 
-    def removeBorder(self):
-        # remove window border
-        if not win_utils.isWin7():
-            self._Form.setWindowFlags(
-                self._Form.windowFlags() | Qt.WindowType.FramelessWindowHint
-            )
+BORDER = 5
+
+
+class FramelessWindow(QWidget):
+    def __init__(self) -> None:
+        super().__init__()
+        self.__background="white"
+        self.__radius=5
+        self.__setupUi()
+        self.__set_frameless()
+        self.__set_animation_toggle()
+
+    def __setupUi(self):
+        self.setLayout(QVBoxLayout())
+        self.layout().setContentsMargins(*([BORDER] * 4))
+        self.layout().setSpacing(0)
+        self.client_window = QWidget(self)
+        self.layout().addWidget(self.client_window)
+        self.titlebar = TitleBar(self)
+        self.main_window = QWidget(self)
+        self.client_window.setLayout(QVBoxLayout())
+        self.client_window.layout().setSpacing(0)
+        self.client_window.layout().setContentsMargins(0, 0, 0, 0)
+        self.client_window.layout().addWidget(self.titlebar)
+        self.client_window.layout().addWidget(self.main_window)
+
+    def __set_frameless(self):
+        self.setWindowFlag(Qt.WindowType.FramelessWindowHint, True)
+        self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground, True)
+        # style sheet
+        self.client_window.setObjectName("__window")
+        self.set_border_radius(BORDER)
+        # resize
+        QCoreApplication.instance().installEventFilter(self)
+
+    def set_border_radius(self, radius: int):
+        self.__radius=radius
+        self.update_stylesheet()
+        
+    def set_theme(self,theme:Theme=Theme.LIGHT,bg_color:str=None):
+        if theme==Theme.LIGHT:
+            self.__background="white" if bg_color is None else bg_color
         else:
-            self._Form.setWindowFlags(
-                Qt.WindowType.FramelessWindowHint
-                | Qt.WindowType.WindowMinMaxButtonsHint
+            self.__background="#383838" if bg_color is None else bg_color
+        self.update_stylesheet()
+        self.titlebar.title.set_theme(theme)
+        self.titlebar.buttons.set_theme(theme)
+        
+    def update_stylesheet(self):
+        self.setStyleSheet(
+            "#__window{background-color:"+str(self.__background)+";border-radius:" + str(self.__radius) + "px;}"
+        )
+
+    def eventFilter(self, obj, event):
+        # resize, refer to https://github.com/zhiyiYo/PyQt-Frameless-Window
+        et = event.type()
+        if et != QEvent.MouseButtonPress and et != QEvent.MouseMove:
+            return False
+        edges = Qt.Edge(0)
+        pos = event.globalPos() - self.pos()
+        if pos.x() < BORDER:
+            edges |= Qt.LeftEdge
+        if pos.x() >= self.width() - BORDER:
+            edges |= Qt.RightEdge
+        if pos.y() < BORDER:
+            edges |= Qt.TopEdge
+        if pos.y() >= self.height() - BORDER:
+            edges |= Qt.BottomEdge
+        # change cursor
+        if et == QEvent.MouseMove and self.windowState() == Qt.WindowNoState:
+            if edges in (Qt.LeftEdge | Qt.TopEdge, Qt.RightEdge | Qt.BottomEdge):
+                self.setCursor(Qt.SizeFDiagCursor)
+            elif edges in (Qt.RightEdge | Qt.TopEdge, Qt.LeftEdge | Qt.BottomEdge):
+                self.setCursor(Qt.SizeBDiagCursor)
+            elif edges in (Qt.TopEdge, Qt.BottomEdge):
+                self.setCursor(Qt.SizeVerCursor)
+            elif edges in (Qt.LeftEdge, Qt.RightEdge):
+                self.setCursor(Qt.SizeHorCursor)
+            else:
+                self.setCursor(Qt.ArrowCursor)
+        elif et == QEvent.MouseButtonPress and edges:
+            self.window().windowHandle().startSystemResize(edges)
+        return False
+
+    def paintEvent(self, event: QPaintEvent) -> None:
+        # set shadow , refer to https://blog.csdn.net/goforwardtostep/article/details/99549750
+        painter = QPainter(self)
+        painter.setRenderHint(QPainter.RenderHint.Antialiasing, True)
+        shadow = QColor(50, 50, 50, 30)
+        for i in range(BORDER):
+            shadow.setAlpha(120 - math.sqrt(i) * 40)
+            painter.setPen(shadow)
+            painter.drawRoundedRect(
+                BORDER - i,
+                BORDER - i,
+                self.width() - (BORDER - i) * 2,
+                self.height() - (BORDER - i) * 2,
+                4,
+                4,
             )
 
-    def addShadowAndAnimatation(self):
-        # add DWM shadow and window animation
-        self.windowEffect.addWindowAnimation(self._Form.winId())
-        if not isinstance(self, AcrylicWindow):
-            self.windowEffect.addShadowEffect(self._Form.winId())
-
-
-class WindowsFramelessWindow(QWidget, Ui_Frameless):
-    """Frameless window for Windows system"""
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self.setupUi(self)
-        self.removeBorder()
-        self.addShadowAndAnimatation()
-        self.setScreenChanged()
-
-    def resizeEvent(self, e):
-        super().resizeEvent(e)
-        self.resizeFrameless()
-
-    def nativeEvent(self, eventType, message):
-        """Handle the Windows message"""
-        return self.nativeFrameless(message)
-
-
-class AcrylicWindow(WindowsFramelessWindow):
-    """A frameless window with acrylic effect"""
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self.__closedByKey = False
-
-        self.setWindowFlags(Qt.WindowType.FramelessWindowHint)
-        self.windowEffect.enableBlurBehindWindow(self.winId())
-        self.windowEffect.addWindowAnimation(self.winId())
-
-        if win_utils.isWin7():
-            self.windowEffect.addShadowEffect(self.winId())
-            self.windowEffect.setAeroEffect(self.winId())
-        else:
-            self.windowEffect.setAcrylicEffect(self.winId())
-            if win_utils.isGreaterEqualWin11():
-                self.windowEffect.addShadowEffect(self.winId())
-
-        self.setStyleSheet("AcrylicWindow{background:transparent}")
-
-    def nativeEvent(self, eventType, message):
-        """Handle the Windows message"""
-        msg = MSG.from_address(message.__int__())
-
-        # handle Alt+F4
-        if msg.message == win32con.WM_SYSKEYDOWN:
-            if msg.wParam == win32con.VK_F4:
-                self.__closedByKey = True
-                QApplication.sendEvent(self, QCloseEvent())
-                return False, 0
-
-        return super().nativeEvent(eventType, message)
-
-    def closeEvent(self, e):
-        if not self.__closedByKey or QApplication.quitOnLastWindowClosed():
-            self.__closedByKey = False
-            return super().closeEvent(e)
-
-        # system tray icon
-        self.__closedByKey = False
-        self.hide()
-
-
-class WindowsFramelessMainWindow(QMainWindow, Ui_Frameless):
-    """Frameless window for Windows system"""
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self.setupUi(self)
-        self.removeBorder()
-        self.addShadowAndAnimatation()
-        self.setScreenChanged()
-
-    def resizeEvent(self, e):
-        super().resizeEvent(e)
-        self.resizeFrameless()
-
-    def nativeEvent(self, eventType, message):
-        """Handle the Windows message"""
-        return self.nativeFrameless(message)
-
-
-class WindowsFramelessFramelessDialog(QDialog, Ui_Frameless):
-    """Frameless dialog"""
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        self.setupUi(self)
-        self.removeBorder()
-        self.addShadowAndAnimatation()
-        self.setScreenChanged()
-        # for dialog
-        self.titleBar.minBtn.hide()
-        self.titleBar.maxBtn.hide()
-        self.titleBar.setDoubleClickEnabled(False)
-
-    def resizeEvent(self, e):
-        super().resizeEvent(e)
-        self.resizeFrameless()
-
-    def nativeEvent(self, eventType, message):
-        """Handle the Windows message"""
-        return self.nativeFrameless(message)
+    def __set_animation_toggle(self):
+        self.__w_normal = 800
+        self.__h_normal = 600
+        self.__animation_toggle = QPropertyAnimation(self, b"geometry")
+        self.__animation_toggle.setStartValue(
+            QRect(self.pos().x(), self.pos().y(), self.__w_normal, self.__h_normal)
+        )
+        self.__animation_toggle.setEndValue(self.get_screen())
+
+    def showMaximized(self,record=True) -> None:
+        if not self.isVisible():
+            self.show()
+        self.titlebar.show()
+        self.layout().setContentsMargins(*([0] * 4))
+        self.set_border_radius(0)
+        if record:
+            self.__h_normal = self.height()
+            self.__w_normal = self.width()
+        self.__animation_toggle.setStartValue(
+            QRect(self.pos().x(), self.pos().y(), self.__w_normal, self.__h_normal)
+        )
+        self.__animation_toggle.setEndValue(self.get_screen())
+        self.__animation_toggle.setDirection(QPropertyAnimation.Direction.Forward)
+        self.__animation_toggle.setDuration(100)
+        self.__animation_toggle.start()
+
+    def showNormal(self) -> None:
+        if not self.isVisible():
+            self.show()
+        self.titlebar.show()
+        self.layout().setContentsMargins(*([BORDER] * 4))
+        self.set_border_radius(BORDER)
+        self.__animation_toggle.setDirection(QPropertyAnimation.Direction.Backward)
+        self.__animation_toggle.start()
+        
+    def showFullScreen(self) -> None:
+        self.titlebar.hide()
+        self.showMaximized()
+
+    def isMaximized(self) -> bool:
+        return self.geometry() == self.get_screen()
+
+    def get_screen(self):
+        rect = self.screen().availableGeometry()
+        rect.setHeight(rect.height() - 2)
+        return rect
+
+    def setWindowIcon(self, icon) -> None:
+        self.titlebar.icon.setIcon(icon)
+        return super().setWindowIcon(icon)
+
+    def setWindowTitle(self, arg__1: str) -> None:
+        self.titlebar.title.setText(arg__1)
+        return super().setWindowTitle(arg__1)
+    
+    def setTitlebar(self,titlebar:QWidget):
+        self.titlebar.deleteLater()
+        self.client_window.layout().replaceWidget(self.titlebar,titlebar)
+        self.titlebar=titlebar
+    
+class FramelessMainWindow(FramelessWindow):
+    def __init__(self) -> None:
+        super().__init__()
+        self.main_window=QMainWindow()
+        
+class FramelessDialog(FramelessWindow):
+    def __init__(self) -> None:
+        super().__init__()
+        self.main_window=QDialog()
+        self.titlebar.buttons.minBtn.hide()
+        self.titlebar.buttons.toggleBtn.hide()
```

### Comparing `QtPy-Frameless-Window-0.0.8/PKG-INFO` & `QtPy-Frameless-Window-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.8
+Version: 0.0.9
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
-Requires-Python: >=3.6
+Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: pyqt
 Project-URL: Homepage, https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 Description-Content-Type: text/markdown
 
@@ -21,24 +21,52 @@
 [![Downloads](https://static.pepy.tech/badge/qtpy-frameless-window)](https://pepy.tech/project/qtpy-frameless-window)
 ![GitHub](https://img.shields.io/github/license/TaoChenyue/Qtpy-Frameless-Window?style=plastic)
 
 A cross-platform frameless window based on QtPy.
 
 </div>
 
-This repo is based on *QtPy* and [PyQt-Frameless-Window](https://github.com/zhiyiYo/PyQt-Frameless-Window). Due to library in diffrent *PyQt-Frameless-Window* branches cannot exist in one virtual environment, I created this repository by adding *QtPy* dependence and modifying some modules. This repo will keep up with *PyQt-Frameless-Window*.
+## Introduce 
+A QWidget/QMainWindow/QDialog is wrapped in another QWidget to realize frameless effect. 
+![structure](assets/structure.png)
+Only qtpy library is required.
 
 ## Install
 To install use pip:
 ```shell
 pip install QtPy-Frameless-Window
 ```
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 pip install -e .
 ```
 
-## FQ
-+ Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
-A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
+## Demo
+QtPy use PyQt5 as default Qt API, so you can run demo with PyQt5 like this.
+```sh
+python examples/dark_demo.py
+python examples/light_demo.py
+```
+Or you can specify your Qt API like this.
+```sh
+python examples/dark_demo.py --api pyside6
+python examples/light_demo.py --api pyqt6
+...
+```
+It is realized by an easy function.
+```python 
+import argparse
+import os
+def set_qt_api(api:str="pyqt5",parse:bool=False):
+    if parse:
+        parser = argparse.ArgumentParser(description='Set Qt API')
+        parser.add_argument('--api', type=str)
+        args = parser.parse_args()
+        if args.api is not None:
+            api=args.api
+    os.environ["QT_API"]=api
+```
+
+![light_demo](assets/light_demo.png)
 
+![dark_demo](assets/dark_demo.png)
```

