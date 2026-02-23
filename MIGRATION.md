# Migration Guide: pythonlover2023 → IrsanAI/LRP-v1.3

## Ziel
Finale Überführung dieses Repositories in das Ziel-Repository:
- **Target:** `https://github.com/IrsanAI/LRP-v1.3`

> Aktueller Sonderfall: Wenn das Quellrepo bereits unter `IrsanAI/...` liegt, ist **kein Owner-Transfer zu `IrsanAI`** möglich/erforderlich. Dann stattdessen im selben Owner nur den Repo-Namen ändern.

## Empfohlene Vorgehensweise

### Option A (bevorzugt, nur bei Owner-Wechsel): Repository Transfer
Nur wenn das Quellrepo noch bei einem *anderen* Owner liegt (z. B. `pythonlover2023/...`) und du Owner-Rechte hast:
1. In GitHub zum Quellrepo gehen → **Settings** → **General**.
2. Ganz unten **Transfer ownership** auswählen.
3. Im Feld **New owner** nur den Owner eintragen (`IrsanAI`) — **nicht** `IrsanAI/LRP-v1.3`.
4. Im separaten Feld **New repository name** den Zielnamen eintragen (`LRP-v1.3`).
5. Transfer bestätigen.

**Wichtig zur UI-Verwirrung:**
- Bei „Select one of my organizations“ wird nur angezeigt, was im aktuell angemeldeten Account verfügbar/zulässig ist.
- Falls `IrsanAI` nicht per Autovervollständigung erscheint, nutze „Specify an organization or username“ und trage dort **nur** `IrsanAI` ein.
- Die Zuordnung zum Zielrepo passiert über das zweite Feld (**New repository name**), nicht über `owner/repo` im Owner-Feld.
- Falls das Zielrepo `IrsanAI/LRP-v1.3` bereits existiert, kann der Transfer mit genau diesem Namen fehlschlagen. Dann entweder Zielrepo vorab löschen/umbenennen oder Option B verwenden.

**Vorteile:**
- Issues, Stars, Watcher, PR-Historie bleiben erhalten.
- Alte URLs werden automatisch umgeleitet.


### Option A1 (wenn Repo schon bei `IrsanAI` liegt): Nur Rename (ohne Transfer)
Wenn dein Repo bereits `IrsanAI/IrsanAI-LRP-v1.3` heißt, dann kommt die GitHub-Meldung
„Repositories cannot be transferred to the original owner“ zurecht.

In diesem Fall ist der korrekte Weg:
1. Im Repo auf **Settings** → **General**.
2. Unter **Repository name** den Namen auf `LRP-v1.3` ändern.
3. Rename bestätigen.

**Warum:**
- Owner bleibt gleich (`IrsanAI`), daher ist ein Transfer zur gleichen Organisation nicht erlaubt.
- Für den Wechsel von `IrsanAI/IrsanAI-LRP-v1.3` → `IrsanAI/LRP-v1.3` reicht ein Rename vollständig aus.

### Option B: Sauberer Neuaufbau + Push
Wenn du bewusst ein frisches Zielrepo nutzen willst:
```bash
# im lokalen Projekt

git remote rename origin legacy

git remote add origin https://github.com/IrsanAI/LRP-v1.3.git

git push -u origin --all

git push origin --tags
```

## Nach der Migration (Checkliste)
- README-Badges/Links auf neues Repo umstellen.
- GitHub Pages in neuem Repo aktivieren.
- Branch Protection & Collaborator-Rollen setzen.
- Legacy-Repo als Archiv/Redirect kennzeichnen.
