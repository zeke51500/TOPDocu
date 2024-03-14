# Testdatei

Dies ist eine Testdatei in Markdown. Hier kannst du verschiedene Markdown-Elemente ausprobieren.

## Überschriften

Du kannst verschiedene Überschriften erstellen, indem du die Anzahl der `#`-Zeichen vor dem Text erhöhst:

# Überschrift der ersten Ebene
## Überschrift der zweiten Ebene
### Überschrift der dritten Ebene

## Aufzählungen

Du kannst Aufzählungen erstellen, indem du `-` oder `*` vor den Listenelementen verwendest:

- Element 1
- Element 2
- Element 3
* Element 4
* Element 5

## Links

Du kannst Links erstellen, indem du den Linktext in eckige Klammern `[]` und die URL in runde Klammern `()` setzt:

[GitHub](https://github.com)

## Codeblöcke

Du kannst Codeblöcke erstellen, indem du den Code zwischen drei Backticks einfügst:
```
app.post("/dashchromadb", (req, res) => {
  let bInsert = true;
  let oChromaInsertData = {
    body: req.body.response,
    prompt: "",
    ab_oder_zusage: "",
    action: "insert",
  };
  console.log("Dash to ChromaDB data: ", req.body);
  sendMailToPythonScript(oChromaInsertData, "", "", bInsert);
  res.send("ChromaDB insert OK. ChromaDB size approximately: " + sLastChromaSize);
});
``` 
