CREATE TABLE `usuarios` (
   `id` INT NOT NULL AUTO_INCREMENT,
   `nombre` VARCHAR(255) NOT NULL,
   `email` VARCHAR(255) NOT NULL,
   PRIMARY KEY (`id`)
);

CREATE TABLE `notas` (
   `id` INT NOT NULL,
   `titulo` VARCHAR(100) NOT NULL,
   `fecha_creacion ` DATE NOT NULL,
   `fecha_modificacion ` DATE NOT NULL,
   `descripcion` TEXT(65535) NOT NULL,
   `eliminable` TINYINT(1) NOT NULL,
   `id_user ` INT NOT NULL,
   PRIMARY KEY (`id`, `id_user `)
);

CREATE TABLE `categorias` (
   `id` INT NOT NULL,
   `nombre` VARCHAR(255) NOT NULL,
   PRIMARY KEY (`id`)
);

CREATE TABLE `registro_categorias` (
   `id` INT NOT NULL,
   `id_nota ` INT NOT NULL,
   `id_categoria` INT NOT NULL,
   PRIMARY KEY (`id`)
);


ALTER TABLE `usuarios` ADD CONSTRAINT `FK_768637b5-8ed2-40db-831b-9b7329b0f00e` FOREIGN KEY (`id`) REFERENCES `notas`(`id`)  ;

ALTER TABLE `registro_categorias` ADD CONSTRAINT `FK_26c25311-55e0-4b2c-a4d7-9aea44a2d8c3` FOREIGN KEY (`id_nota `) REFERENCES `notas`(`id`)  ;

ALTER TABLE `registro_categorias` ADD CONSTRAINT `FK_6ddb06ca-361b-448b-9cc1-ef06f5e41c82` FOREIGN KEY (`id`) REFERENCES `categorias`(`id`)  ;
