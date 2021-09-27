# dbAutomotriz
base de datos de automotriz

create database Automotriz

use automotriz

create table Linea_Montaje(
 idLinea_montaje int primary key not null
)

create table modelo(
 idmodelo int primary key not null,
 nombre varchar(45)
)

create table estacion(
 idestacion int primary key not null,
 orden int
)

create table automovil(
 numero_chasis varchar(45) primary key not null,
 patente varchar(45),
 fecha_finalizacion datetime
)

create table pedido(
 numero int primary key not null,
 fecha_hora datetime
)

create table tarea(
 idTarea int primary key not null,
 nombre varchar(45)
)

create table insumo (
 codigo_insumo int primary key not null,
 descripcion_insumo varchar(45),
 precio_insumo float
)

create table concesionario (
 id_concesionario int primary key not null,
 nombre varchar(45),
 direccion varchar(45),
 telefono varchar(45)
)

create table provedor (
 id_concesionario int primary key not null,
 nombre varchar(45),
 direccion varchar(45),
 telefono varchar(45)
)

create table compra (
 numero_compra int primary key not null,
 fecha datetime
)
