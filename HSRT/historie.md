# Historie – HSRT WV/Thesis

> Chronologisches Decision-Log über alle Rollen hinweg.
> Neueste Einträge oben, direkt unter dieser Linie.
> Ein Eintrag pro Arbeitssitzung. Knapp halten: Entscheidungen
> und offene Punkte, kein Gesprächsprotokoll.

---

## 2026-05-16 | Rolle: Setup

**Thema:** Aufsetzen einer rollenübergreifenden Projekthistorie und
Klärung eines Multi-Agent-Workflows.

**Entscheidungen:**
- Multi-Agent-Ansatz: pro Rolle ein eigenes Claude-Project als Einstieg;
  echtes Agent-Zusammenspiel nur über API/Framework, vorerst nicht verfolgt.
- Historie-Strategie: Option A — manuell. Claude erzeugt am Sitzungsende
  einen Markdown-Eintrag, der Nutzer committet ihn selbst ins Repo.
- Eine gemeinsame `historie.md` für alle Rollen, nicht je Rolle eine
  Datei. Rolle steht in der Eintrags-Kopfzeile.
- Eintragsformat festgelegt: Datum | Rolle, dann Thema, Entscheidungen,
  Ergebnisse/Artefakte, Offene Punkte, Nächster Schritt.

**Ergebnisse/Artefakte:**
- Ergänzungsblock "Project History & Log Identity" für `WV/Role_WV.md`.
- Ergänzungsblock "Project History & Context" für `Plan/Role_planer.md`
  (deckt MyAdvisor und MyManager ab; nennt rahmenbedingungen.md,
  profile.md, Role_WV.md, historie.md als Kontextquellen).
- Diese Datei `HSRT/historie.md`.

**Offene Punkte:**
- Trigger `MyAdvisor` erweitern, sodass er alle vier Kontext-Files fetcht
  statt nur `Role_planer.md`? — unentschieden.
- Eigenen Trigger `MyHistory` für `historie.md` in die Preferences
  aufnehmen? — unentschieden.
- "Context Sources"-Abschnitt auch für `Role_WV.md` ergänzen, damit beide
  Rollen symmetrisch sind? — unentschieden.
- Inhaltliche Konvention: ist `Setup` ein dauerhaft erlaubter Rollen-Tag
  neben MyAdvisor/MyManager/MyResearcher? — zu klären.

**Nächster Schritt:** Nutzer committet `historie.md` und die zwei
Ergänzungsblöcke ins Repo; offene Trigger-Fragen in einer der nächsten
Sitzungen entscheiden.

---