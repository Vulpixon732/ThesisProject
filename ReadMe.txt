Algorytm dynamicznego generowania scenerii dostosowującego się do etapu gry oraz wyników gracza - Pliki źródłowe
Konrad Wargin, 29291

[SPIS TREŚCI]
1. Wstęp;
2. Wymagane programy;
3. Instalacja UE5;
4. Uruchomienie projektu;
5. Inspekcja kodu;
6. Sterowanie - Edytor Blueprint;
7. Uruchomienie gry;
8. Sterowanie - Prototyp gry;
9. Instrukcja gry;
10. Lista plików zawierających kod bezpośrednio związany z tematem pracy.

[1. Wstęp]
Projekt został wykonany wykorzystując język Blueprint Visual Scripting w silniku Unreal Engine 5.3.2, z tego powodu kod istnieje w formie plików binarnych. Aby odczytać kod programu, należy otworzyć edytor z poziomu silnika Unreal Engine 5.3.2.

[2. Wymagane programy]
- Epic Games Launcher (Wymagane konto Epic Games);
- Unreal Engine 5.3.2;
Rekomendowane wymagania sprzętowe:
System Operacyjny:  Windows 10 64-bit wersja 1909, lub wersje 2004 and 20H2 lub nowsze.
Procesor:  Quad-core Intel or AMD, 2.5 GHz lub szybszy.
Pamięć: 32 GB RAM
GPU RAM:   8 GB lub więcej.
Karta graficzna:  Karta graficzna kompatybilna z DirectX 11 or 12.

[3. Instalacja UE5]
1. Należy zainstalować aplikację Epic Games Launcher z pliku 'EpicInstaller-18.5.0-unrealEngine.msi' lub pobrać instalator ze strony https://www.unrealengine.com/en-US/download;
2. Po instalacji należy uruchomić Epic Games Launcher i zalogować się (Konto jest wymagane do pobrania silnika);
3. W Epic Games Launcher przejść na zakładkę Unreal Engine i podstronę Biblioteka;
4. W kategorii "Wersje silnika" nacisnąć ikonę +, nacisnąć na liczbę w widocznym obiekcie poniżej i wybrać "5.3.2";
5. Po wybraniu wersji należy nacisnąć "Zainstaluj".

[4. Uruchomienie projektu]
1. Należy uruchomić Epic Games Launcher i zalogować się;
2. W Epic Games Launcher przejść na zakładkę Unreal Engine i podstronę Biblioteka;
3. W kategorii "Wersje silnika" wybrać przycisk "Uruchom" pod silnikiem z wersją "5.3.2";
4. Po uruchomieniu silnika należy wybrać kategorię "Recent projects" i nacisnąć przycisk "Browse...";
5. W wyborze pliku należy otworzyć plik "ThesisProject.uproject";
6. W wypadku jeżeli pojawi się informacja o wymaganym przebudowaniu plików należy zatwierdzić przebudowanie plików.

[5. Inspekcja kodu]
1. Aby zobaczyć pliki projektowe należy otworzyć "Content Drawer" w dolnym lewym rogu edytora;
2. Aby otworzyć edytor pliku należy podwójnie nacisnąć Lewy Przycisk Myszy na wybrany plik lub nacisnąć Prawy Przycisk Myszy na wybranym pliku i wybrać "Edit..." z menu kontekstowego;
2a. Jeżeli edytor pliku otworzy się w formie "Data Only Blueprint", w górnej części okna w zdaniu "NOTE: This is data only blueprint, so only default values are shown. It does not have any script or variables. If you want to add some, Open Full Blueprint Editor" należy nacisnąć "Open Full Blueprint Editor";
3. Po otwarciu okna edytora z wybranym plikiem, funkcje oraz zmienne można znaleźć w zdokowanym oknie "My Blueprint";
3a. W wypadku jeżeli okno "My Blueprint" nie jest widoczne w edytorze, należy z paska narzędzi na górze edytora wybrać "Window/My Blueprint";
4. Aby otworzyć edytor Blueprint należy podwójnie nacisnąć Lewy Przycisk Myszy na wybranej Funkcji lub Grafie, lub nacisnać Prawy Przycisk Myszy na wybranej Funkcji lub Grafie i wybrać "Open Graph";
5. Szczegóły funkcji oraz zmiennych takie jak wartości domyślne oraz zmienne wejściowe/wyjściowe funkcji znajdują się w zdokowanym oknie "Details";
5a. W wypadku jeżeli okno "Details" nie jest widoczne w edytorze, należy z paska narzędzi na górze edytora wybrać "Window/Details";
6. Dołączone komponenty przy klasach będącymi aktorami na scenie znajdują się w zdokowanym oknie "Components";
6a. W wypadku jeżeli okno "Components" nie jest widoczne w edytorze, należy z paska narzędzi na górze edytora wybrać "Window/Components".

[6. Sterowanie - Edytor Blueprint]
Lewy Przycisk Myszy - Wybór bloku kodu;
Przytrzymanie Lewego Przycisku Myszy - Wybór grupowy bloków kodu;
Przytrzymanie Lewego Przycisku Myszy (Z wybranym blokiem kodu) - Przesunięcie bloku kodu;
Prawy Przycisk Myszy - Menu dodania nowego bloku kodu;
Przytrzymanie Prawego Przycisku Myszy - Przesuwanie kamery edytora grafów;
Przytrzymanie Prawego Przycisku Myszy (Kursor na bloku kodu) - Otworzenie menu kontekstowego bloku;
Kółko myszy - Przybliżenie kamery edytora grafów.

[7. Uruchomienie gry]
1. Należy przejść do okna edytora sceny (Edytor otwiera domyślnie mapę MAP_DebugThesis);
2. W pasku narzędzi nad podglądem sceny, należy nacisnąć "Change Play Mode and Play Settings" (ikona ⋮) i wybrać tryb uruchomienia gry (Rekomendowane "New Editor Window (PIE)");
3. W pasku narzędzi nad podglądem sceny, należy nacisnąć "Play" lub użyć skrótu klawiszowego [Alt+P].

[8. Sterowanie - Prototyp gry]
A - Ruch w Lewo;
D - Ruch w Prawo;
L - Skok;
J - Atak.

[9. Instrukcja gry]
Celem gracza w prototypie jest pokonanie wszystkich wygenerowanych przeciwników na mapie.
Pokonany przeciwnik zmienia wygląd modelu postaci na wersje leżącą.
Po pokonaniu wszystkich przeciwników, aby przejść do następnego losowo generowanego etapu, gracz musi przejść na prawy dolny róg mapy i wejść w miejsce oznaczone znacznikami "LE" (Level Exit).

[10. Lista plików zawierających kod bezpośrednio związany z tematem pracy]
Content/Blueprints/BP_LevelEnd.uasset;
Content/Blueprints/GI_Thesis.uasset;
Content/Blueprints/GM_Thesis.uasset;
Content/Blueprints/Characters/Shark/BP_Shark.uasset;
Content/Blueprints/Structs/S_TileInfo.uasset;
Content/Maps/MAP_DebugThesis.umap;
Content/Maps/PrototypeMaps/*;
Content/PaperAssets/TileSets/Markers/*;
Content/PaperAssets/TileSets/TileMaps/TM_Layout1.uasset;
Content/PaperAssets/TileSets/TileMaps/TM_Layout2.uasset;
Content/PaperAssets/TileSets/TileMaps/TM_Layout3.uasset;
Content/PointSystem/**.