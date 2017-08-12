# Data Provinsi, Kota/Kabupaten, Kecamatan, dan Kelurahan/Desa di Indonesia
Data ini diambil dari situs [Pemutakhiran MFD dan MBS
Badan Pusat Statistik (http://mfdonline.bps.go.id/)](http://mfdonline.bps.go.id/) pada **12 Agustus 2017**.

# Administrative Subdivisions of Indonesia (Provinces, Regencies/Cities, Districts, Villages)
The data were taken from [Central Agency on Statistics (BPS) - MFD and MBS Update (http://mfdonline.bps.go.id/)](http://mfdonline.bps.go.id/) on **12 Agustus 2017**.

The data were `curl`-ed from BPS site:

    curl http://mfdonline.bps.go.id/index.php?link=hasil_pencarian --data "pilihcari=desa&kata_kunci="
    
with `a`, `i`, `u`, `e` and `o` as the keywords.

## Statistics

+------+---------------------------+----------------+-----------+----------------+
| Kode | Provinsi                  | Kabupaten/Kota | Kecamatan | Desa/Kelurahan |
+------+---------------------------+----------------+-----------+----------------+
| 11   | ACEH                      |             23 |       289 |           6509 |
| 12   | SUMATERA UTARA            |             33 |       443 |           6113 |
| 13   | SUMATERA BARAT            |             19 |       179 |           1117 |
| 14   | RIAU                      |             12 |       169 |           1876 |
| 15   | JAMBI                     |             11 |       141 |           1562 |
| 16   | SUMATERA SELATAN          |             17 |       232 |           3261 |
| 17   | BENGKULU                  |             10 |       129 |           1520 |
| 18   | LAMPUNG                   |             15 |       228 |           2643 |
| 19   | KEPULAUAN BANGKA BELITUNG |              7 |        47 |            391 |
| 21   | KEPULAUAN RIAU            |              7 |        70 |            416 |
| 31   | DKI JAKARTA               |              6 |        44 |            267 |
| 32   | JAWA BARAT                |             27 |       627 |           5963 |
| 33   | JAWA TENGAH               |             35 |       573 |           8559 |
| 34   | DI YOGYAKARTA             |              5 |        78 |            438 |
| 35   | JAWA TIMUR                |             38 |       666 |           8501 |
| 36   | BANTEN                    |              8 |       155 |           1551 |
| 51   | BALI                      |              9 |        57 |            716 |
| 52   | NUSA TENGGARA BARAT       |             10 |       116 |           1141 |
| 53   | NUSA TENGGARA TIMUR       |             22 |       307 |           3323 |
| 61   | KALIMANTAN BARAT          |             14 |       174 |           2074 |
| 62   | KALIMANTAN TENGAH         |             14 |       136 |           1574 |
| 63   | KALIMANTAN SELATAN        |             13 |       152 |           2008 |
| 64   | KALIMANTAN TIMUR          |             10 |       103 |           1032 |
| 65   | KALIMANTAN UTARA          |              5 |        53 |            482 |
| 71   | SULAWESI UTARA            |             15 |       171 |           1838 |
| 72   | SULAWESI TENGAH           |             13 |       175 |           2019 |
| 73   | SULAWESI SELATAN          |             24 |       307 |           3054 |
| 74   | SULAWESI TENGGARA         |             17 |       220 |           2330 |
| 75   | GORONTALO                 |              6 |        77 |            735 |
| 76   | SULAWESI BARAT            |              6 |        69 |            650 |
| 81   | MALUKU                    |             11 |       118 |           1236 |
| 82   | MALUKU UTARA              |             10 |       115 |           1195 |
| 91   | PAPUA BARAT               |             13 |       189 |           1622 |
| 94   | PAPUA                     |             29 |       567 |           4924 |
+------+---------------------------+----------------+-----------+----------------+
```

```

## Generate new data

In order to generate new data:

    cd scripts
    pip install -r requirements.txt
    ./run.sh

You can also run `docker-compose` (more preferred):

    docker-compose build
    docker-compose up

## License

* The scripts are license under: [MIT](license.md).
* The data (CSV and SQL) are under: [ODBL v1.0](odbl-10.md).
* The source data is attributed to **Badan Pusat Statistik (BPS) Indonesia**.

## Contributing

1. Fork it (https://github.com/edwardsamuel/Wilayah-Administratif-Indonesia/fork).
2. Create your feature branch (`git checkout -b my-new-feature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin my-new-feature`).
5. Create a new Pull Request.
