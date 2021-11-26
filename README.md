# ReallySmartButelki

## Konfiguracja

Do konfiguracji niezbędny jest docker oraz zbudowanie obrazu dostępnego w folderze docker:
1. Przejdź do folderu docker
2. Uruchom komendę: `docker build . -t tensorflow-with-scipy`
3. Do uruchomienia wywołaj komendę: `docker run -it --rm -p 8888:8888 -v $PWD:/notebook/ -m=1000m tensorflow-with-scipy`
4. W konsoli pojawi ci się link do notatnika jupyter

