The latest release version <a href="https://github.com/bonecode/TBCEditor/releases">1.9.0</a>

Use the Issues page to report bugs or send them directly to lasse@bonecode.com.

<h3>Description</h3>

A syntax highlighting edit control for RAD Studio (Delphi/C++ Builder) with code folding, completion proposal, matching pair, minimap, sync edit, multi-caret editing, word wrap, support for non-fixed-width fonts, etc. External highlighter and color scheme files are in JSON format which can be also loaded from a stream.

<h3>Build requirements</h3>

* <a href="https://github.com/ahausladen/JsonDataObjects">Json Data Objects</a> (included)
* Delphi versions XE4-8, Seattle, and Berlin are supported 
* C++ Builder versions XE7-8, Seattle, and Berlin are supported

<b>Note!</b> Do not offer me older versions to support. I don't have time to keep up with those.

<h3>Conditional compilation</h3>

Define | Description 
--- | --- 
USE_ALPHASKINS | Use <a href="http://www.alphaskins.com/">AlphaSkins</a>. AlphaSkins are most powerful theming solutions for apps developed in Delphi.
USE_VCL_STYLES | Use VCL styles. A set of graphical details that define the look and feel of a VCL application.

<h3>Usage example</h3>

```objectpascal
  with BCEditor1 do 
  begin
    Highlighter.LoadFromFile('JSON.json');
    Highlighter.Colors.LoadFromFile('Default.json'); 
    LoadFromFile(GetHighlighterFileName('JSON.json')); 
    ...
    Lines.Text := Highlighter.Info.General.Sample; 
  end;
```
<b>Note!</b> LoadFromStream does not support multi-highlighters (for example HTML with Scripts.json). Override TBCBaseEditor.CreateFileStream function, if you want to load multi-highlighters from a stream. 

<h3>Demo</h3>

TBCEditor Control Demo v. 2.0.0 (dev).

  * <a href="http://www.bonecode.com/downloads/BCEditorComponentDemo32.zip">32-bit Windows</a>
  * <a href="http://www.bonecode.com/downloads/BCEditorComponentDemo64.zip">64-bit Windows</a>

The latest update: 05.02.2017 20:19, UTC+02:00

<h3>Documentation</h3>

Documentation will be written after the project stabilizes and dust settles. This project is developed in my spare time without sources of income and as long as this is the case there is no timetable for anything. 

<h3>Projects using the control</h3>

* <a href="http://www.bonecode.com">EditBone</a>
* <a href="http://www.mitec.cz/ibq.html">MiTeC Interbase Query</a>
* <a href="http://www.mitec.cz/sqliteq.html">MiTeC SQLite Query</a>

<h3>Screenshots</h3>

![bceditor0](https://cloud.githubusercontent.com/assets/11475177/20067778/2e403442-a51f-11e6-8c3e-532ae48b7d72.png)
![bceditor1](https://cloud.githubusercontent.com/assets/11475177/20067780/2e5c78be-a51f-11e6-98b3-837ab6c630f9.png)
![bceditor2](https://cloud.githubusercontent.com/assets/11475177/20067783/2e7e074a-a51f-11e6-9152-e7298b510fac.png)
![bceditor3](https://cloud.githubusercontent.com/assets/11475177/20067782/2e7e15b4-a51f-11e6-945f-69ae5f7c6391.png)
![bceditor4](https://cloud.githubusercontent.com/assets/11475177/20067784/2e7e457a-a51f-11e6-802d-1b90bd952538.png)
![bceditor5](https://cloud.githubusercontent.com/assets/11475177/20114666/d317c5a0-a5fd-11e6-9c0d-8fc71d177943.png)
![bceditor6](https://cloud.githubusercontent.com/assets/11475177/20067785/2e831d16-a51f-11e6-93ca-51eb13a1501f.png)
![bceditor7](https://cloud.githubusercontent.com/assets/11475177/20067786/2e83a9c0-a51f-11e6-918d-e039512503ca.png)
![bceditor8](https://cloud.githubusercontent.com/assets/11475177/20067774/2de408c0-a51f-11e6-9bbc-68c4824c7d10.png)
![bceditor9](https://cloud.githubusercontent.com/assets/11475177/20067777/2e22d398-a51f-11e6-80dc-aada64961860.png)









