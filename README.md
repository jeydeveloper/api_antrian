# api_antrian
API Antrian

## URL END POINT:
--------------------------------------

- GET /v1/transaksi/sisa/:addressCaller [TESTING]

- GET /v1/transaksi/next/:addressCaller [TESTING]

- GET /v1/transaksi/status/:addressCaller [ONPROGRESS]

- GET /v1/transaksi/recall/:addressCaller [ONPROGRESS]

- GET /v1/transaksi/skip/:addressCaller [ONPROGRESS]

- GET /v1/transaksi/finish/:addressCaller [ONPROGRESS]

- GET /v1/transaksi/nextManual/:addressCaller [ONPROGRESS]


## KONFIGURASI DATABASE:
--------------------------
File config ada di file "root/config/database.php"


## SAMPLE URL:
----------------

1. 	Request URL : http://localhost/api_antrian/v1/transaksi/next/1

	Response Server :
	----------------------------------
	{
	    "code": 200,
	    "message": "Result is empty!"
	}
	----------------------------------

2. 	Request URL : http://localhost/api_antrian/v1/transaksi/sisa/1

	Response Server :
	----------------------------------
	{
	    "code": 200,
	    "result": {
	        "jumlah": 0
	    }
	}
	----------------------------------