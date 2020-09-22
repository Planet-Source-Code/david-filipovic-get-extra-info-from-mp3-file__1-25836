<div align="center">

## Get extra info from MP3 file


</div>

### Description

Explains which bytes are used, and how, to store info about bit-rate, frequency, channels...
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[David Filipovic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/david-filipovic.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Sound/MP3](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/sound-mp3__1-45.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/david-filipovic-get-extra-info-from-mp3-file__1-25836/archive/master.zip)





### Source Code

<HTML>
<HEAD>
<META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=windows-1252">
<TITLE>Untitled Document</TITLE>
<STYLE type="text/css">
  div {font-family:Verdana; font-size:8pt} .dejvi {font-family:Verdana; font-size:8pt; color:red}
</STYLE></HEAD>
<BODY>
<CENTER>
<FONT CLASS="dejvi">
2nd byte has to be in between [F2,F7] or [FA,FF],<BR>
and the info extracted from 2nd byte is as follows:<BR><BR>
</FONT>
<CENTER><TABLE BORDER CELLSPACING=1 CELLPADDING=1 WIDTH=200>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Value </div></TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG, Layer</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">CRC</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">F2</div> </TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">F3</div> </TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">F4</div> </TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0, Layer 2</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">F5</div> </TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0, Layer 2</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">F6</div> </TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0, Layer 1</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">F7</div> </TD>
<TD WIDTH="70%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0, Layer 1</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
</TABLE>
</CENTER>
&nbsp;
<CENTER><TABLE BORDER CELLSPACING=1 CELLPADDING=1 WIDTH=200>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Value </div></TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG, Layer</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">CRC</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">FA</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">FB</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">FC</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">FD</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">FE</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">FF</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0, Layer 3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
</TABLE>
</CENTER>
<BR>
<FONT CLASS="dejvi">
3rd byte has to be in between [1x,Fx] (Where x is between [0,B]),<BR>
and the info extracted from 3rd byte is as follows:<BR><BR>
</FONT>
<CENTER><TABLE BORDER CELLSPACING=1 CELLPADDING=1 WIDTH=200>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Value (x)</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0 Frequency</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0 Frequency</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">[0,3]</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">44 KHz</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">22 KHz</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">[4,7]</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">48 KHz</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">24 KHz</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">[8,B]</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">32 KHz</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">16 KHz</div> </TD>
</TR>
</TABLE>
</CENTER>
<BR>
<CENTER><TABLE BORDER CELLSPACING=1 CELLPADDING=1 WIDTH=200>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Value</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">MPEG 1.0 Bit-rate</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">MPEG 2.0 Bit-rate</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">1x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">32 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">8 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">2x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">40 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">16 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">3x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">48 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">24 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">4x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">56 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">32 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">5x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">64 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">40 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">6x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">80 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">48 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">7x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">96 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">56 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">8x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">112 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">64 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">9x</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">128 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">80 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Ax</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">160 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">96 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Bx</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">192 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">112 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Cx</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">224 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">128 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Dx</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">256 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">144 Kbit</div> </TD>
</TR>
<TR><TD WIDTH="20%" VALIGN="MIDDLE">
<div align="center">Ex</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">320 Kbit</div> </TD>
<TD WIDTH="40%" VALIGN="MIDDLE">
<div align="center">160 Kbit</div> </TD>
</TR>
</TABLE>
</CENTER>
<BR>
<FONT CLASS="dejvi">
4rd byte is of type ax(hex), where a is between [0,F], and x is between [0,F],<BR>
and the info extracted from 3rd byte is as follows:<BR><BR>
</FONT>
<CENTER><TABLE BORDER CELLSPACING=1 CELLPADDING=1 WIDTH=250>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Value (a)</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Original</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">Emphasis</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Copyright</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">0</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">None</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">1</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">50/15 microsec</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">2</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">Invalid</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">3</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">CITT j. 17</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">4</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">None</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">5</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">50/15 microsec</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">6</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">Invalid</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">7</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">CITT j. 17</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE" HEIGHT=18>
<div align="center">8</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE" HEIGHT=18>
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE" HEIGHT=18>
<div align="center">None</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE" HEIGHT=18>
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">9</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">50/15 microsec</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">A</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">Invalid</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">B</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">No</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">CITT j. 17</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">C</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">None</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">D</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">50/15 microsec</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">E</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">Invalid</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">F</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
<TD WIDTH="80%" VALIGN="MIDDLE">
<div align="center">CITT j. 17</div> </TD>
<TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Yes</div> </TD>
</TR>
</TABLE>
</CENTER>
<BR>
<CENTER><TABLE BORDER CELLSPACING=1 CELLPADDING=1 WIDTH=130>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">Value (x)</div> </TD>
<TD WIDTH="90%" VALIGN="MIDDLE">
<div align="center">Channels</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">[0,3]</div> </TD>
<TD WIDTH="90%" VALIGN="MIDDLE">
<div align="center">Stereo</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">[4,7]</div> </TD>
<TD WIDTH="90%" VALIGN="MIDDLE">
<div align="center">Joint Stereo</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">[8,B]</div> </TD>
<TD WIDTH="90%" VALIGN="MIDDLE">
<div align="center">2 Channels</div> </TD>
</TR>
<TR><TD WIDTH="10%" VALIGN="MIDDLE">
<div align="center">[C,F]</div> </TD>
<TD WIDTH="90%" VALIGN="MIDDLE">
<div align="center">Mono</div> </TD>
</TR>
</TABLE>
</CENTER>
</CENTER>
</BODY>
</HTML>

