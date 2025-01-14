# make-mermaid-swim-by-db
make mermaid ER code from db (python)

# Require
- Python3.10
- sqlalchemy
- mysqlclient
- **your (mysql)DB**

# usage
- install
```
pip install DB2mermaid
```

- use
```
from db2mermaid.db2mermaid import DB2Mermaid
    dm = DB2Mermaid()
    dm.init_db("user", "pasword", "127.0.0.1", "3306", "db_name")
    dm.generate()
```

then, you will get `er.md`

### Output Sample of Skila
ref: https://downloads.mysql.com/docs/sakila-db.tar.gz

![output sapmle](./images/skila-sample.png)

[mermaid live editor](https://mermaid.live/edit#pako:eNqtV9GOojAU_RXSpzExE0FB8c0ZcdeMuhPH2exsTEwDxWkChZQyOy7x3_cC4qIWxM3yBJy255zbe28hQXbgEDREhI8p3nLsr5kCF7ZFwJP8Pr1e5qPZbLpY5cCGOsrz01_0-2j5-HW0vOvpLcWlPBIbhn0ixz18Aa-mc-tlNZo_52AcOlgAvD9IcRxOokgqJoeq5OidVjGkFtQuUQ1Qh0aCU1tIiG0qdinrRMKqwtQwiAT2Nmls5WuH7wErQYvX2UzxAhsLGrCmgUlFJDXiqkKS4rJpQcwEv7B1RUM-Kalfr1JJPqQxGTxsgxO21XTxlpEdoCo2DTLvlqSz40gEPpGWQIGdcxVaAOWkKjv-sUTKUSM-pl59NUwksqBy6UdpyfFoZaVBUGxOwPom998sPJnFpMa6LC4-ZngLYYPScN1zlddd1OuBJaV6DlT_sVtdU_ow-_aghNA3Yt5sA2vzpmr3jt3GaClxRHiFhbTV4Cj6FXCnaSxd6vmytE_fV4VS1QYtRVDhlTPI-rFSHBLZnIanbe3NGi0VTjyCI7LZEcwv7XqYbWPIlqpwBJxuKYMWe20gJyztxE7Mz3rr2HqcgrW73kZrFaP4SQkcnXuEbcX75VQ9nxp62CY-rAD9PiqdFtbida6ktGxbWtSCjQ6JTYHOhbqDJIma7kzhNamPV3mDjgfOLc0v2-nbvgBqs6QBm6S1X1myvu83oBTkU9ya55quN8jzAwtlH5AUp6bm1nj6Ok9pjujVUE6eGveKOtMh3qVJKrN8gCqVlE88uRpJRwfA-mIti9o6Q09qCPvph4DkaCqE3XI25XxJnZCyySNX0SlOqCr2a3JLlEoMUO7swkxNDKucojYCIjhGHPh0z6yukXiHJrRGQ7h1iItjT6xRPjSfZjkU5KOhi72ItBGORfCyY_bxRT7q8BdwfBtihoYJ-kTDXue-bxqGafa7ar9ndHp6G-3QUDXV-87A0LqGbupad6AO9m30OwhgCfXe6Hc0zTS6qto3O6rZbyOSqZjnPx3Zv0fG8TObIHhM9n8AOUymUQ)

# Caution ❗
this package is not full.
It cannot generate table relation, can only generate table definition 😢.
(And now, only mysql... 🤣)

# Future
Make CLI