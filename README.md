# covid19 bot

## Config

- Update the file config/default.js
- More info https://github.com/lorenwest/node-config

## Database Script

- create `covid19ec` schema
- create `msp` table

```sql
CREATE TABLE `msp` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `anio` int(11) DEFAULT NULL,
  `cod_prov_res` varchar(10) DEFAULT NULL,
  `prov_residencia` varchar(100) DEFAULT NULL,
  `cod_cant_res` varchar(10) DEFAULT NULL,
  `cant_residencia` varchar(100) DEFAULT NULL,
  `sexo` varchar(10) DEFAULT NULL,
  `edad` int(11) DEFAULT NULL,
  `tipo_edad` varchar(10) DEFAULT NULL,
  `grupo_edad` varchar(20) DEFAULT NULL,
  `inicio_sintomas` date DEFAULT NULL,
  `diagnostico` varchar(200) DEFAULT NULL,
  `condicion_paciente` varchar(10) DEFAULT NULL,
  `clasificacion_caso` varchar(50) DEFAULT NULL,
  `total_muestras` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`)
)
```

## Run

```bash
npm start
```

## Output

- `source` folder - imported data
- `target` folder - exported data
