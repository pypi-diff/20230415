# Comparing `tmp/pyees-1.1.5.tar.gz` & `tmp/pyees-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.1.5.tar", last modified: Fri Apr 14 08:24:40 2023, max compression
+gzip compressed data, was "pyees-1.1.6.tar", last modified: Sat Apr 15 19:35:00 2023, max compression
```

## Comparing `pyees-1.1.5.tar` & `pyees-1.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:24:20.703124 pyees-1.1.5/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      616 2023-04-14 08:24:20.718749 pyees-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 08:24:20.468747 pyees-1.1.5/pyees/
--rw-rw-rw-   0        0        0      619 2023-03-30 05:48:48.000000 pyees-1.1.5/pyees/__init__.py
--rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.5/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.5/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.5/pyees/prop.py
--rw-rw-rw-   0        0        0    14265 2023-04-14 07:44:37.000000 pyees-1.1.5/pyees/readData.py
--rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.5/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.5/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.5/pyees/testFit.py
--rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.5/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-14 07:48:34.000000 pyees-1.1.5/pyees/testPyees.py
--rw-rw-rw-   0        0        0     9133 2023-04-03 11:24:36.000000 pyees-1.1.5/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.5/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8532 2023-04-14 08:02:12.000000 pyees-1.1.5/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.1.5/pyees/testVariable.py
--rw-rw-rw-   0        0        0    43260 2023-04-14 07:59:45.000000 pyees-1.1.5/pyees/unit.py
--rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.1.5/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:24:20.656248 pyees-1.1.5/pyees.egg-info/
--rw-rw-rw-   0        0        0      616 2023-04-14 08:24:18.000000 pyees-1.1.5/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-14 08:24:19.000000 pyees-1.1.5/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:24:18.000000 pyees-1.1.5/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-14 08:24:18.000000 pyees-1.1.5/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 08:24:19.000000 pyees-1.1.5/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-14 08:24:20.749999 pyees-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-14 08:24:09.000000 pyees-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:35:00.739427 pyees-1.1.6/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      616 2023-04-15 19:35:00.745410 pyees-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:35:00.561901 pyees-1.1.6/pyees/
+-rw-rw-rw-   0        0        0      619 2023-03-30 05:48:48.000000 pyees-1.1.6/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.6/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.6/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.6/pyees/prop.py
+-rw-rw-rw-   0        0        0    14263 2023-04-15 19:33:22.000000 pyees-1.1.6/pyees/readData.py
+-rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.6/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.6/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.6/pyees/testFit.py
+-rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.6/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-14 07:48:34.000000 pyees-1.1.6/pyees/testPyees.py
+-rw-rw-rw-   0        0        0     9335 2023-04-15 19:33:08.000000 pyees-1.1.6/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.6/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.1.6/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.1.6/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.1.6/pyees/unit.py
+-rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.1.6/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:35:00.719480 pyees-1.1.6/pyees.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-04-15 19:34:59.000000 pyees-1.1.6/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-15 19:34:59.000000 pyees-1.1.6/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:34:59.000000 pyees-1.1.6/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-15 19:34:59.000000 pyees-1.1.6/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 19:35:00.727459 pyees-1.1.6/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-15 19:35:00.770344 pyees-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-15 19:34:54.000000 pyees-1.1.6/setup.py
```

### Comparing `pyees-1.1.5/LICENSE.txt` & `pyees-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/PKG-INFO` & `pyees-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.5
+Version: 1.1.6
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.5/README.md` & `pyees-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/__init__.py` & `pyees-1.1.6/pyees/__init__.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/fit.py` & `pyees-1.1.6/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/profilePyees.py` & `pyees-1.1.6/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/prop.py` & `pyees-1.1.6/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/readData.py` & `pyees-1.1.6/pyees/readData.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,8 +353,7 @@
 ## TODO change the name of "readData" to "sheetFromFile"
 ## TODO read data vælg ark
 ## TODO the inputs of "sheetFromFile" has to be able to take list-list inputs and return a list of Sheets
 ## TODO save Sheet as xlFile
 
 ## TODO error when reading from multiple sheets with different number of rows
 
-
```

### Comparing `pyees-1.1.5/pyees/solve.py` & `pyees-1.1.6/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/stackOverflowODR.py` & `pyees-1.1.6/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/testFit.py` & `pyees-1.1.6/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/testProp.py` & `pyees-1.1.6/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/testPyees.py` & `pyees-1.1.6/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/testReadData.py` & `pyees-1.1.6/pyees/testReadData.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         np.testing.assert_array_equal(dat1.s1.a.uncert, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
         np.testing.assert_array_equal(dat1.s1.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
         self.assertEqual(str(dat1.s1.b.unit), 'mA')
         np.testing.assert_array_equal(dat1.s1.b.uncert, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
 
         dat4 = readData('testData/data4.xlsx', 'A-B')
         dat5 = readData('testData/data5.xlsx', 'A-B')
+    
         with self.assertRaises(Exception) as context:
             dat4.s1.append(dat5.s1)
         self.assertTrue("You can only append sheets with the excact same measurements. The names did not match" in str(context.exception))
 
         dat3 = readData('testData/data3.xlsx', 'A-B')
         dat4 = readData('testData/data4.xlsx', 'A-B')
         with self.assertRaises(Exception) as context:
@@ -147,10 +148,15 @@
                     self.assertEqual(str(meas.unit), 'L/min')
                     np.testing.assert_array_equal(meas.uncert, [0, 0, 0, 0, 0])
                 else:
                     np.testing.assert_array_equal(meas.value, [5, 6, 7, 8, 9])
                     self.assertEqual(str(meas.unit), 'mA')
                     np.testing.assert_array_equal(meas.uncert, [0, 0, 0, 0, 0])
 
+    def testNontypeInput(self):
+        dat = readData("testData/data7.xlsx", "A-F")
+        for sheet in dat:
+            for elem in sheet:
+                self.assertEqual(elem.unit, '1')
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyees-1.1.5/pyees/testSolve.py` & `pyees-1.1.6/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/testUnit.py` & `pyees-1.1.6/pyees/testUnit.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,17 @@
         a = unit('L/min')
         with self.assertRaises(Exception) as context:
             converter = a.getConverter('m')
         self.assertEqual('You tried to convert from L/min to m. But these do not have the same base units', str(context.exception))
 
     def testInput(self):
 
+        a = unit(None)
+        self.assertEqual(str(a), '1')
+        
         a = unit('m / s')
         self.assertEqual(str(a), 'm/s')
 
         with self.assertRaises(Exception) as context:
             a = unit('m!/s')
         self.assertEqual('The character ! is not used within the unitsystem', str(context.exception))
 
@@ -182,20 +185,29 @@
             a = unit('m/s/bar')
         self.assertEqual('A unit can only have a single slash (/)', str(context.exception))
 
         self.assertEqual(str(unit(' ')), '1')
         self.assertEqual(str(unit('-')), '1')
         self.assertEqual(str(unit('')), '1')
         self.assertEqual(str(unit('--')), '1')
+        self.assertEqual(str(unit('- -')), '1')
+        
         self.assertEqual(str(unit('()')), '1')
         self.assertEqual(str(unit('( )')), '1')
         self.assertEqual(str(unit('(  )')), '1')  
         self.assertEqual(str(unit('(-)')), '1')
         self.assertEqual(str(unit('(--)')), '1')
+        self.assertEqual(str(unit('(- -)')), '1')
         self.assertEqual(str(unit('( -)')), '1')
+        self.assertEqual(str(unit('( - (- ))')), '1')
+        
+        
+        self.assertEqual(str(unit('(m/s2)2/Hz')), 'm2/s4-Hz')
+        self.assertEqual(str(unit('(m1/s2)2/Hz')), 'm2/s4-Hz')
+        self.assertEqual(str(unit('(m1/s2)1/Hz')), 'm/s2-Hz')
 
     def testAddNewUnit(self):
         addNewUnit('gnA', 9.81, 'm/s2')
         converter = unit('gnA').getConverter('m/s2')
         self.assertEqual(converter.convert(1), 9.81)
         
         addNewUnit('gnB', 9.81, 'm/s2', 0)
@@ -224,13 +236,12 @@
         
         converter = unit('Ra').getConverter('K')
         self.assertAlmostEqual(converter.convert(83.1), 46.1666666666666666666667)
         
         converter = unit('Ra').getConverter('Rø')
         self.assertAlmostEqual(converter.convert(83.1), -111.66625)
         
-        
-        
-        
+
+    
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyees-1.1.5/pyees/testVariable.py` & `pyees-1.1.6/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees/unit.py` & `pyees-1.1.6/pyees/unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             raise Warning(f'The unit {item} known in more than one unit system')
 
 
 
 # determine the known characters within the unit system
 knownCharacters = list(knownUnits.keys()) + list(knownPrefixes.keys())
 knownCharacters = ''.join(knownCharacters)
-knownCharacters += '-/'
+knownCharacters += '-/ '
 knownCharacters += '0123456789'
 knownCharacters += '()'
 knownCharacters = set(knownCharacters)
 
 # check if all unit and prefix combinations can be distiguished
 unitPrefixCombinations = []
 for u in knownUnits:
@@ -507,132 +507,179 @@
             upper = ['DELTA' + elem if elem in temperature else elem for elem in upper]
             lower = ['DELTA' + elem if elem in temperature else elem for elem in lower]
 
         return upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp
 
     @ staticmethod
     def _formatUnit(unitStr):
-        ## TODO this is a mess - remake this
-
-        # Removing any spaces
-        unitStr = unitStr.replace(' ', '')
-
+        
+        if unitStr is None:
+            return '1'
+        
         # Removing any illegal symbols
         for s in unitStr:
             if s not in knownCharacters:
                 raise ValueError(f'The character {s} is not used within the unitsystem')
 
         ## find start parenthesis is the unit string
         startParenIndexes = [i for i, s in enumerate(unitStr) if s == '(']
         stopParenIndexes = [i for i, s in enumerate(unitStr) if s == ')']
 
         ## return if no parenthesis where found
         if not startParenIndexes and not stopParenIndexes:
-            return unitStr
-      
+            return unit.__formatUnit(unitStr)
+        
         ## check that the number of start and stop parenthesis are equal
         if len(startParenIndexes) != len(stopParenIndexes):
-            raise ValueError('The unit string has to have an equal number of open parenthesis and clsoe parenthesis')
+            raise ValueError('The unit string has to have an equal number of open parenthesis and close parenthesis')
+        
+        if len(startParenIndexes) == 1 and startParenIndexes[0] == 0 and stopParenIndexes[0] == len(unitStr) -1:
+            return unit._formatUnit(unitStr[startParenIndexes[0]+1:stopParenIndexes[0]])
         
         ## find all parenthesis pairs
         allIndexes = startParenIndexes + stopParenIndexes
         allIndexes.sort()
         isStartParen = [elem in startParenIndexes for elem in allIndexes]
-        done, iter, maxIter, order  = False, 0, len(allIndexes), []
+        done, iter, maxIter, parenOrder  = False, 0, len(allIndexes), []
         while not done:
             for i in range(len(allIndexes)-1):
                 if isStartParen[i] and (isStartParen[i] + isStartParen[i+1] == 1):
-                    order.append([allIndexes[i], allIndexes[i+1]])
+                    parenOrder.append([allIndexes[i], allIndexes[i+1]])
                     allIndexes.pop(i+1)
                     allIndexes.pop(i)
                     isStartParen.pop(i+1)
                     isStartParen.pop(i)
                     break
 
             if len(allIndexes) == 0: break
             
             iter += 1
             if iter > maxIter:
                 raise ValueError('An order to evaluate the parenthesis could not be found')
         
+        parenOrder.append([0,len(unitStr)])
+        
+        for i in range(len(parenOrder)-1):
+            currentParens = parenOrder[i]
+            nextParens = parenOrder[i+1]
+            end = currentParens[1]
+            
+            _unitStr = unitStr[currentParens[0]+1:currentParens[1]]
+            _unitStrLenOriginal = len(_unitStr)
+            _unitStr = unit._formatUnitStringWithParenthesis(_unitStr)
+            if nextParens[0] <= currentParens[0] and nextParens[1]>=currentParens[1]:
+                nextBit = unitStr[currentParens[1]+1:nextParens[1]]
+                exponent = nextBit.split('/')[0]
+                exponent = exponent.split('-')[0]
+                
+                try:
+                    exponent = int(exponent)
+                    upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp = unit._getLists(_unitStr)
+                    siBaseUnit = unit._getSIBaseUnit(upper, upperExp ,lower, lowerExp)
+                    _unitStr = unit.__staticPow(_unitStr, upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp, siBaseUnit, exponent)[0]
+                    end += len(str(exponent))
+                except ValueError: pass
+            
+            _unitStrLenUpdate = len(_unitStr)
+            
+            dLen = _unitStrLenUpdate - _unitStrLenOriginal
+            for j in range(i, len(parenOrder)):
+                if parenOrder[j][0] >= currentParens[1]: parenOrder[j][0] += dLen
+                if parenOrder[j][1] >= currentParens[1]: parenOrder[j][1] += dLen-1
+            
+            unitStr = unitStr[0:currentParens[0]] + '(' + _unitStr + ')' + unitStr[end+1:]
 
-        ## find the outer most parenthesis        
-        done, maxIter, iter = False, len(order), 0
+    
+        unitStr = unit._formatUnitStringWithParenthesis(unitStr)
+        
+        ## find start parenthesis is the unit string
+        startParenIndexes = [i for i, s in enumerate(unitStr) if s == '(']
+        stopParenIndexes = [i for i, s in enumerate(unitStr) if s == ')']
+        
+        ## check that the number of start and stop parenthesis are equal
+        if len(startParenIndexes) != len(stopParenIndexes):
+            raise ValueError('The unit string has to have an equal number of open parenthesis and close parenthesis')
+        
+        if len(startParenIndexes) == 0:
+            return unitStr
+        
+        done = False
         while not done:
-            changesMade = False
-            for i in range(len(order)):
-                iLow = order[i][0]
-                iHigh = order[i][1]
-                for j in range(len(order)):
-                    jLow = order[j][0]
-                    jHigh = order[j][1]
-                    if iLow < jLow and iHigh > jHigh:
-                        order.pop(j)
-                        changesMade = True
-                        break
-                if changesMade:
-                    break
-            if not changesMade:
+            if unitStr[0] == '(' and unitStr[len(unitStr)-1] == ')':
+                unitStr = unitStr[1:len(unitStr)-1]
+            else:
                 break
-            iter += 1
-            if iter > maxIter:
-                raise ValueError('An order to evaluate the parenthesis could not be found')
         
-        ## find all slashes outside the outer most parenthesis
-        slashes = [i for i, s in enumerate(unitStr) if s == slash]
-
-        iter, maxIter, done = 0, len(slashes), False
-        while not done:
-            done = True
-            for s in slashes:    
-                for part in order:
-                    if part[0] < s < part[1]:
-                        done = False
-                        slashes.remove(s)
-                        break                
-            if done: break
-            iter += 1
-            if iter > maxIter:
-                raise ValueError('An order to evaluate the parenthesis could not be found')
+        if '(' in unitStr or ')' in unitStr:    
+            raise ValueError('The unit could not be parsed')
+        
+        return unitStr
 
-        if len(slashes) > 1:
-            raise ValueError('You have more than one slash ("/") outside the outer most parenthesis. This makes the unit ambiguis')
+    
+    @staticmethod
+    def _formatUnitStringWithParenthesis(unitStr):
         
-        if slashes:
-            splits = [-1] + slashes
-            parts = [unitStr[i+1:j] for i,j in zip(splits, splits[1:]+[None])]
-            parts = [unit._formatUnit(part) for part in parts]
-            if isinstance(parts, list):
-                parts = unit(parts[0]) / unit(parts[1])
-            return parts
-        
-        parts = unit._formatUnit(unitStr[order[0][0]+1: order[0][1]])
-        if order[0][1] != len(unitStr) - 1:
-            remaining = unitStr[order[0][1]+1:]
-            parts = parts.split('/')
-            if len(parts) > 1:
-                upper, lower = parts
-                lower = lower.split('-')
-            else:
-                upper, lower = parts[0], []
-            upper = upper.split('-')
-            try: 
-                exponent = int(remaining)
-                for i, up in enumerate(upper):
-                    u, e = unit._removeExponentFromUnit(up)
-                    upper[i] = u + str(e * exponent)
-                for i, low in enumerate(lower):
-                    u, e = unit._removeExponentFromUnit(low)
-                    lower[i] = u + str(e * exponent)
-                out = '-'.join(upper)
-                if lower:
-                    out += '/' + '-'.join(lower)
-            except TypeError:
-                raise TypeError()
-        return parts
+        ## determine if there is a slash outside of a parenthesis pair
+        tally = 0
+        for i, s in enumerate(unitStr):
+            if s == '/' and tally == 0:
+                
+                a = unitStr[0:i]
+                b = unitStr[i+1:]
+                a = unit._formatUnit(a)
+                b = unit._formatUnit(b)
+                
+                aUpper, aUpperPrefix, aUpperExp, aLower, aLowerPrefix, aLowerExp = unit._getLists(a)
+                bUpper, bUpperPrefix, bUpperExp, bLower, bLowerPrefix, bLowerExp = unit._getLists(b)
+                
+                upper = aUpper + bLower
+                upperPrefix = aUpperPrefix + bLowerPrefix
+                upperExp = aUpperExp + bLowerExp
+                lower = aLower + bUpper
+                lowerPrefix = aLowerPrefix + bUpperPrefix
+                lowerExp = aLowerExp + bUpperExp
+                
+                return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix ,lowerExp)
+            
+            if s == '(':
+                tally += 1
+            if s == ')':
+                tally -= 1
+      
+        
+        return unit.__formatUnit(unitStr)
+        
+    
+            
+    @staticmethod
+    def __formatUnit(unitStr):
+        # Removing any spaces
+        unitStr = unitStr.replace(' ', '')
+        unitStr = unitStr.split('/')
+        
+        if len(unitStr)>2:
+            raise ValueError('A unit can only have a single slash (/)')
+        
+        if len(unitStr) > 1:
+            upper, lower = unitStr
+            lower = [elem for elem in lower.split('-') if elem != '']
+        else:
+            upper, lower = unitStr[0], []
+        
+        upper = [elem for elem in upper.split('-') if elem != '']
+        
+        if upper:
+            out = '-'.join(upper)
+        else:
+            out = '1'
+        
+        if lower:
+            out += '/' + '-'.join(lower)
+            
+        return out
     
     @ staticmethod
     def _splitCompositeUnit(compositeUnit):
         lower = []
         if not slash in compositeUnit:
             upper = compositeUnit.split(hyphen)
             return upper, lower
@@ -928,15 +975,14 @@
         if self._SIBaseUnit == other._SIBaseUnit:
             return isLogarithmicUnit, self._SIBaseUnit, True, False, False
         
         
         
         raise ValueError(f'You tried to subtract a variable in [{other}] from a variable in [{self}], but the units do not have the same SI base unit')
 
-
     def __mul__(self, other):
         return unit._multiply(self.unitStr, other.unitStr)
 
     def __truediv__(self, other):
         
         a = self.unitStr
         b = other.unitStr
@@ -951,74 +997,77 @@
             lowerPrefix=bUpperPrefix,
             lowerExp=bUpperExp
         )
 
         return unit._multiply(a, b)
 
     def __pow__(self, power):
+        return self.__staticPow(self.unitStr, self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp, self._SIBaseUnit, power)
+    
+    @staticmethod
+    def __staticPow(unitStr, upper, upperPrefix, upperExp ,lower, lowerPrefix, lowerExp, _SIBaseUnit, power):
         if power == 0:
             return '1', False
 
         elif power > 1:
 
-            if self.unitStr == '1':
+            if unitStr == '1':
                 # self is '1'. Therefore the power does not matter
-                return self.unitStr, False
+                return unitStr, False
 
             else:
                 # self is not '1'. Therefore all exponents are multiplied by the power
 
                 if not (isinstance(power, int) or power.is_integer()):
                     raise ValueError('The power has to be an integer')
 
-                upperExp = [int(elem * power) for elem in self.upperExp]
-                lowerExp = [int(elem * power) for elem in self.lowerExp]
+                upperExp = [int(elem * power) for elem in upperExp]
+                lowerExp = [int(elem * power) for elem in lowerExp]
 
-                return self._combineUpperAndLower(self.upper, self.upperPrefix, upperExp, self.lower, self.lowerPrefix, lowerExp) , False
+                return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp) , False
 
         else:
             # the power is smaller than 1.
             # Therefore it is necessary to determine if all exponents are divisible by the recibricol of the power
 
-            if self.unitStr == '1':
+            if unitStr == '1':
                 # self is '1'. Therefore the power does not matter
-                return self.unitStr, False
+                return unitStr, False
             else:
                 # self is not '1'.
                 # Therefore it is necessary to determine if all exponents are divisible by the recibricol of the power
 
                 def isCloseToInteger(a, rel_tol=1e-9, abs_tol=0.0):
                     b = np.around(a)
                     return abs(a - b) <= max(rel_tol * max(abs(a), abs(b)), abs_tol)
                 
                 # Test if the exponent of all units is divisible by the power
                 try:
-                    for exp in self.upperExp + self.lowerExp:
+                    for exp in upperExp + lowerExp:
                         if not isCloseToInteger(exp * power):
-                            raise ValueError(f'You can not raise a variable with the unit {self.unitStr} to the power of {power}')
+                            raise ValueError(f'You can not raise a variable with the unit {unitStr} to the power of {power}')
 
-                    upperExp = [int(elem * power) for elem in self.upperExp]
-                    lowerExp = [int(elem * power) for elem in self.lowerExp]
+                    upperExp = [int(elem * power) for elem in upperExp]
+                    lowerExp = [int(elem * power) for elem in lowerExp]
 
-                    return self._combineUpperAndLower(self.upper, self.upperPrefix, upperExp, self.lower, self.lowerPrefix, lowerExp), False
+                    return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp), False
                 
                 except ValueError:                
                     ## the exponents of the unit was not divisible by the power
                     ## test if the exponents of the SIBaseunit is divisible by the power 
                     
-                    siUpper, siUpperPrefix, siUpperExp, siLower, siLowerPrefix, siLowerExp = self._getLists(self._SIBaseUnit)
+                    siUpper, siUpperPrefix, siUpperExp, siLower, siLowerPrefix, siLowerExp = unit._getLists(_SIBaseUnit)
                     for exp in siUpperExp + siLowerExp:
                         if not isCloseToInteger(exp * power):
-                            raise ValueError(f'You can not raise a variable with the unit {self.unitStr} to the power of {power}')
+                            raise ValueError(f'You can not raise a variable with the unit {unitStr} to the power of {power}')
 
                     siUpperExp = [int(elem * power) for elem in siUpperExp]
                     siLowerExp = [int(elem * power) for elem in siLowerExp]
 
-                    return self._combineUpperAndLower(siUpper, siUpperPrefix, siUpperExp, siLower, siLowerPrefix, siLowerExp), True
-
+                    return unit._combineUpperAndLower(siUpper, siUpperPrefix, siUpperExp, siLower, siLowerPrefix, siLowerExp), True
 
     def getConverter(self, newUnit):
         newUnit = unit._formatUnit(newUnit)
 
         # get the upper, upperExp, lower and lowerExp of the newUnit without creating a unit
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(newUnit)
 
@@ -1097,15 +1146,12 @@
 
         self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
         self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
 
 
 if __name__ == "__main__":
-    a = unit(' ')
-    print(a)
-    a = unit('-')
-    print(a)
-    a = unit('')
-    print(a)
+    
+    print(unit('((s/m6)2)'))
+
```

### Comparing `pyees-1.1.5/pyees/variable.py` & `pyees-1.1.6/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.5/pyees.egg-info/PKG-INFO` & `pyees-1.1.6/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.5
+Version: 1.1.6
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.5/setup.py` & `pyees-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.1.5',
+    version='1.1.6',
     license='MIT',
     description='EES but for python',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

