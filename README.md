# Konwencja Nazewnicza ( #TYDZIEN3.1 )

- Obowiązującym językiem nazewniczym jest język angielski
- Wszelkie nazwy piszemy małymi literami
- Obowiązuje alfabet angielski oraz cyfry 0-9
- Znak '-' może być użyty tylko w miejscu występowania we wzorze
- Wygenerowana nazwa musi być unikatowa

# Zasady nazewnictwa dla zasobów
## Formuły dostępne w nazwach
Poniższe formuły w wzorach nazw należy podmienić na odpowiednie projektowi wartości.

- `<prefix>` - Unikalny 3 znakowy prefix projektu (np. fei)
- `<env>` - Identyfikator środowiska od 3 do 5 znaków (np. dev, prod, uat)
- `<name>` - Nazwa określająca usługę bądz cel lub context zasobu od 3 do maksymalnej długości nazwy określonej w tabeli (maksymalna długość nazwy zawiera wszystkie znaki w wzorze)
- `<index>` - Index zasobu jeśli istnieje wiecej niż 1 zasób o tej samej nazwie dozwolone tylko cyfry

## Wzory nazw dla zasobów

| Zasób | Wzór | Maksymalna długość pełnej wygenerowanej nazwy |
| :---| :---|:---|
|Resource Group| `<prefix>-<env>-rg-<name>` | 90|
|Virtual Network| `<prefix>-<env>-vnet-<name><index>` | 64|
|Subnet| `<prefix>-<env>-snet-<name><index>`| 80
|Network Interface|`<prefix>-<env>-nic-<name><number>`|80
|Public IP|`<prefix>-<env>-pip-<name>`|80
|NSG|`<prefix>-<env>-nsg-<name>`|80
|Virtual Machine| `<prefix>-<env>-vm-<name><index>` |1–15 (Windows), 1–64 (Linux)|
|Disks| `<prefix><env>disk<name><number>` | 24
|Storage| `<prefix><env>stg<name><index>`| 24|