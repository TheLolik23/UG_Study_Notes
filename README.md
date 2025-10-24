# Tutorial jak robić notatki w kilka osób i tego nie rozjebać

## Przygotowanie środowiska

1. Zainstaluj [GITa](https://git-scm.com/install/) w wersji z GUI. Jeżeli już macie legitymację studencką to polecam [Git Kraken](https://www.gitkraken.com/download), ale dowolny inny też będzie GIT.
2. Zainstaluj [Obsidiana](https://obsidian.md/download)
3. [Utwórz forka](https://github.com/TheLolik23/UG_Study_Notes/fork) głównego repo
4. Klonujemy nowo utworzone repo na nasz komputer (poprzez aplikacje, która wybraliście w kroku 1)
5. Otwieramy w Obsidianie folder z repo jako Vault

### Polecane wtyczki społeczności

| Wtyczka                                                                                 | Funkcjonalność                                       |
| --------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| [obsidian-latex-suite](https://obsidian.md/plugins?id=obsidian-latex-suite)             | Uproszczenie używania LaTeX do zapisu matematycznego |
| [obsidian-excalidraw-plugin](https://obsidian.md/plugins?id=obsidian-excalidraw-plugin) | Edytowanie i podgląd rysunków w Excalidraw           |
| [code-styler](https://obsidian.md/plugins?id=code-styler)                               | Ulepszone formatowanie kodu                          |
| [obsidian-icon-folder](https://obsidian.md/plugins?id=obsidian-icon-folder)             | Dostępność ikon                                      |

## Informacje

W zależności od tego czy planujecie uczestniczyć w tej inicjatywie biernie czy aktywnie musicie wybrać odpowiedni Branch.

### Dostępne branche

| Branch      | Przeznaczenie                                             |
| ----------- | --------------------------------------------------------- |
| main        | Pełne notatki już gotowe do nauki                         |
| to_check    | Notatki już skończone gotowe do dodania do main'a         |
| in_progress | Notatki częściowo zrobione, jeszcze nie w pełni skończone |

### Struktura projektu

```text
.
├── Semestr 1.md
└── Notatki
    └── Dziedzina 1
        └── Przedmiot 1
            ├── Przedmiot 1.md
            ├── Ćwiczenia
            │   ├── Przedmiot - Ćwiczenia
            │   └── Przedmiot - Ćw 1.md
            └── Wykłady
                ├── Przedmiot - Wykłady.md
                └── Przedmiot - W 1.md
```

- Każdy przedmiot posiada MOC w której zawarte są inforacje o ECTS, zasadach zaliczenia, i formach zajęć w jakich jest realizowany
- Każda forma zajęć przedmiotu posiada MOC w której zawarte są informacje o prowadzącym, ewenetualncyh zasadach zaliczenia danych zajęć, oraz podlinkowane są notatki z zajęć
- Przedmioty podlinkowane są w MOC danego semestru

### Jak dodawać notatki

Jeśli stworzyliście jakieś nowe notatki to:

1. Upewnijcie się że są zgodne z tym co było do teraz:
   - są w odpowiednim folderze
   - użyty jest odpowiedni template
   - dane w sekcji 'properties' są wypełnione
   - użyte linki działają i odnoszą do odpowiednich notatek
2. Jeśli nie wykonaliście tego co jest napisane powyżej -> to GG bo ja będę musiał to poprawiać, więc wykonajcie krok powyżej
3. Zrób pusha commitów do twojego forka
4. Utwórz na Githubie Pull Request do odpowiedniego brancha głównego repo. Dwa razy w tygodniu będę sprawdzał push requesty i dodawał wasze notatki.

## Leksykon pojęć

- **MOC _(Map of Content)_** - notatka, która jest łącznikiem kontekstowym pomiędzy innymi notatkami
