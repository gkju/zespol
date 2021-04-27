# Aplikacja zespół

# Uruchamianie serwera:

---
### Wymagania:
    - docker
    - docker-compose
### Proces na windows:

---
W powershellu:
```powershell
docker-compose -f .\docker-compose-windows.yml build
docker-compose -f .\docker-compose-windows.yml up
```

### Proces na linux:

---
```powershell
docker-compose -f ./docker-compose-linux.yml build
docker-compose -f ./docker-compose-linux.yml up
```

# Uruchamianie klienta:

---

## Wersja skompilowana na Windows x64

### Wymagania
    - windows x64

Wystarczy otworzyć folder i uruchomić ZespolKlient.exe

## Samodzielna kompilacja/uruchamianie

### Wymagania
    - .net5.0
    - windows x64

Aplikacja klient jest projektem csproj znajdującym się w /ZespolWpfGui, zależnie od narzędzi różnie wygląda uruchamianie, przy użyciu .net cli wystarczy używać dotnet restore, build, run, publish

# Używanie

Aby dodać serwer wystarczy otworzyć okno zarządzania serwerami/nacisnąć dodaj serwer 
i domyślnie wprowadzić serwer o adresie url http://localhost:5000 (dla takiej konfiguracji serwera jak w dostarczonych plikach)

**Ważne: Zawsze należy uwzględnić protokół (tutaj zawsze http, obecnie https nie działa również dla wersji docker-compose-linux)**
~~localhost:5000~~\
**http://localhost:5000 OK (origin)**\
**http://localhost:5000/ OK (url)** 