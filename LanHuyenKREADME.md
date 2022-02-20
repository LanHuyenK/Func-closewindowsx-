Local $var = WinList()
	For $i = 1 To $var[0][0]
		If $var[$i][0] <> "" AND isvisible($var[$i][1]) Then
			If StringRegExp($var[$i][0], "Brave") Then WinClose($var[$i][0])
			Sleep(200)
		EndIf
	Next
EndFunc
