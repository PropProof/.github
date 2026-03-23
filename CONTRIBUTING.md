​
# 🚀 Contributing to PropProof

Wir nutzen GitHub-Automatisierungen, um Zeit zu sparen und Fehler zu vermeiden. Bitte halte dich an diesen Prozes.

## 🛠 1. Aufgaben starten

Erstelle Branches **niemals manuell** lokal. Nutze die GitHub UI:

1. **Issue wählen:** Gehe ins `planning` Repo und suche dir ein Issue aus.
2. **Assignee:** Weise dir das Issue selbst zu (`Assignees` -> `me`).
3. **Branch erstellen:** Klicke rechts in der Sidebar unter "Development" auf **"Create a branch"**.
   * **Vorteil:** GitHub benennt den Branch automatisch nach der Issue-ID (z.B. `1-neues-login-feature`).
   * **Vorteil:** Das Issue wird im Project Board automatisch in **"In Progress"** verschoben.
   * **Vorteil:** Das Issue ist direkt mit dem Branch verknüpft.

## 💻 2. Lokal arbeiten

Hole dir den automatisch erstellten Branch auf deinen Rechner:
```bash
git fetch origin
git checkout <branch-name-aus-github>
```

## 🔄 3. Pull Requests (PR) & Auto-Close

​Sobald du fertig bist, erstelle einen Pull Request.

​Verknüpfung: Nutze in der PR-Beschreibung das Keyword closes #<Issue-Nummer>.

​Automatisierung: Sobald der PR in den main gemergt wird, schließt GitHub das Issue automatisch und schiebt es im Projektboard auf "Done".

## ​🔍 4. Code Quality & Reviews

​Status Checks: Bevor du jemanden um ein Review bittest, müssen die GitHub Actions (Linter/Tests) "grün" sein.

​Review: Weise mindestens ein Teammitglied als Reviewer zu.

​Konversationen: Alle Kommentare im Code müssen als "Resolved" markiert sein, bevor der Merge-Button aktiv wird.

## 🛑 5. Schutzregeln

​Der main-Branch ist geschützt. Direkte Pushes werden vom System abgelehnt. Nur via PR und mit mindestens einem Approval ist ein Merge möglich.
