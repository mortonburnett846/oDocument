# oDocument
sleep(5000) consolewrite("Action 7 retrieve document after clicking a hyperlink" &amp; @CRLF)     findThemAll($oDocument,$treescope_subtree)      $oForumLink=_UIA_getObjectByFindAll($oDocument,"name:=Forum", $treescope_subtree)     if not isobj($oForumLink) Then         findThemAll($oDocument,$treescope_subtree)     EndIf     _UIA_action($oForumLink,"invoke")     sleep(3000)
