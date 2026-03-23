​
# 📋 Checkliste: Neues Repository erstellen

​Dieses Dokument dient als Leitfaden, um sicherzustellen, dass jedes neue Projekt innerhalb von PropProof von Anfang an professionell konfiguriert ist.

## 1. Grundeinstellungen
- [ ] Repository Name: Kleingeschrieben, mit Bindestrichen (z.B. mvp-frontend).
- [ ] ​Sichtbarkeit: Korrekt setzen (Private für Code, Public für das .github Konfig-Repo).
- [ ] README.md: Initialisieren mit Projektname, Kurzbeschreibung und Quick-Start Guide.
- [ ] .gitignore: Passend zum Tech-Stack hinzufügen (z.B. Node, Python, etc.).

## 2. Struktur & Verknüpfung

- [ ] Project Board: Das Repo dem Haupt-Projektboard der Organisation zuweisen.

- [ ] Teams: Schreibzugriff für das Team @propproof/dev gewähren.

## 3. Branch Protection (WICHTIG)

​Gehe zu Settings > Branches > Add branch protection rule:

- [ ] Branch name pattern: main
- [ ] Require a pull request before merging: Aktivieren.
- [ ] Required approvals: Mindestens 1.
- [ ] Dismiss stale pull request approvals: Aktivieren.
- [ ] Require conversation resolution before merging: Aktivieren.
- [ ] Block force pushes: Aktivieren.

## 4. Automatisierung (CI/CD)
- [ ] Workflow Dateien: Ordner .github/workflows/ erstellen.
- [ ] Linting: lint.yml hinzufügen (siehe Vorlage in .github).
- [ ] Testing: test.yml hinzufügen.
- [ ] Status Checks: In den Branch Protection Rules die Checks lint und test als verpflichtend markieren (erst möglich, nachdem die Actions einmal gelaufen sind).

## ​5. Security & Maintenance
- [ ] Dependabot: Unter Settings > Code security and analysis aktivieren (Grouped Version Updates).
- [ ] Secret Scanning: Sicherstellen, dass Secret Scanning aktiviert ist.
- [ ] CODEOWNERS: Datei im Root erstellen und Hauptverantwortliche für Reviews eintragen.

## 6. Development Workflow
- [ ] Issue Templates: Prüfen, ob die globalen Templates aus dem .github Repo korrekt angezeigt werden.
- [ ] Development Section: Testweise einen Branch über ein Issue erstellen, um die Automatisierung zum Projektboard zu prüfen.
