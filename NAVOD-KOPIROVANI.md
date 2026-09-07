# Návod: Jak zkopírovat HTML podpis do Gmailu a Apple Mailu

## 📧 Gmail

### Metoda 1: Přímé vložení HTML (doporučeno)
1. Otevřete soubor `signature-michal.html` nebo `signature-honza.html` v textovém editoru
2. **Vyberte celý obsah** (Cmd+A / Ctrl+A)
3. **Zkopírujte** (Cmd+C / Ctrl+C)
4. V Gmailu:
   - Klikněte na **⚙️ Nastavení** (vpravo nahoře)
   - Přejděte na **Všechna nastavení**
   - V sekci **Obecné** najděte **Podpis**
   - Klikněte na **+ Vytvořit nový** nebo upravte existující
   - V editoru podpisu klikněte na ikonu **</>** (Zobrazit HTML)
   - **Vložte zkopírovaný HTML kód** (Cmd+V / Ctrl+V)
   - Klikněte na **OK** nebo **Uložit změny**

### Metoda 2: Přes prohlížeč
1. Otevřete soubor HTML v prohlížeči (Safari, Chrome, Firefox)
2. **Zobrazte zdrojový kód stránky** (Cmd+Option+U / Ctrl+U)
3. Najděte a zkopírujte obsah `<table>` tagu (od řádku 9 do konce)
4. Vložte do Gmailu podle Metody 1

---

## 📬 Apple Mail (macOS)

### Metoda 1: Přes HTML editor
1. Otevřete soubor `signature-michal.html` nebo `signature-honza.html` v textovém editoru
2. **Vyberte celý obsah** (Cmd+A)
3. **Zkopírujte** (Cmd+C)
4. V Apple Mail:
   - Otevřete **Mail** > **Předvolby** (Cmd+,)
   - Přejděte na záložku **Podpisy**
   - Vyberte účet nebo klikněte na **+** pro vytvoření nového
   - Klikněte na **+** pod seznamem podpisů
   - V pravém panelu klikněte pravým tlačítkem do textového pole
   - Vyberte **Vložit jako HTML** nebo **Paste and Match Style**
   - Pokud nefunguje, použijte Metodu 2

### Metoda 2: Přes prohlížeč (nejspolehlivější)
1. Otevřete soubor HTML v **Safari** (ne Chrome!)
2. **Zobrazte zdrojový kód** (Cmd+Option+U)
3. Najděte a zkopírujte obsah od `<table>` tagu (od řádku 9)
4. V Apple Mail:
   - Otevřete **Mail** > **Předvolby** > **Podpisy**
   - Vytvořte nebo upravte podpis
   - Vložte zkopírovaný kód (Cmd+V)
   - Apple Mail by měl automaticky rozpoznat HTML

### Metoda 3: Přes Rich Text Editor
1. Otevřete soubor HTML v **Safari**
2. **Zkopírujte celou stránku** (Cmd+A, Cmd+C) přímo z prohlížeče
3. V Apple Mail:
   - Otevřete **Mail** > **Předvolby** > **Podpisy**
   - Vytvořte nebo upravte podpis
   - Vložte (Cmd+V) - Apple Mail by měl zachovat formátování

---

## ⚠️ Důležité poznámky

- **Obrázky musí být online**: Podpisy používají obrázky z `https://semicolon.cz/signature/` - ujistěte se, že jsou tyto soubory dostupné na serveru
- **UTF-8 kódování**: Podpisy obsahují meta tag pro UTF-8, takže české znaky (á, é, í, ó, ú, ý, č, ď, ě, ň, ř, š, ť, ž) by se měly zobrazovat správně
- **Testování**: Po vložení pošlete testovací e-mail sobě a zkontrolujte, jak vypadá
- **Zálohování**: Před změnou existujícího podpisu si ho zkopírujte
- **Gmail**: Pokud se podpis zobrazí špatně, zkuste znovu kliknout na **</>** a zkontrolovat HTML

---

## 🔧 Řešení problémů

### Gmail zobrazuje HTML kód jako text
- Ujistěte se, že jste klikli na ikonu **</>** (Zobrazit HTML) před vložením
- Zkuste vložit kód znovu

### Apple Mail nezobrazuje obrázky
- Zkontrolujte, že jsou obrázky dostupné na `https://semicolon.cz/signature/`
- Otevřete URL obrázku v prohlížeči a ověřte, že se načítá

### Podpis se rozpadá v mobilních klientech
- To je normální - mobilní klienti mají omezenou podporu HTML
- Desktopové klienty by měly zobrazovat podpis správně

### České znaky se zobrazují špatně
- Podpisy obsahují meta tag pro UTF-8 kódování
- Pokud se znaky stále zobrazují špatně, zkontrolujte, že kopírujete celý obsah včetně meta tagu na začátku
- Ujistěte se, že váš textový editor ukládá soubory v UTF-8 (většina moderních editorů to dělá automaticky)
