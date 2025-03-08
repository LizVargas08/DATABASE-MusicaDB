-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Servidor: 127.0.0.1
-- Tiempo de generación: 08-03-2025 a las 20:50:35
-- Versión del servidor: 10.4.32-MariaDB
-- Versión de PHP: 8.2.12

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Base de datos: `musicadb`
--

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `canciones`
--

CREATE TABLE `canciones` (
  `id_cancion` int(11) NOT NULL,
  `titulo` varchar(100) NOT NULL,
  `duracion` time NOT NULL,
  `id_genero` int(11) NOT NULL,
  `idioma` varchar(50) NOT NULL,
  `id_artista` int(11) NOT NULL,
  `id_album` int(11) DEFAULT NULL,
  `tempoBPM` int(11) DEFAULT NULL,
  `esInstrumental` tinyint(1) DEFAULT NULL,
  `calificacion` decimal(3,2) DEFAULT NULL,
  `reproducciones` int(11) DEFAULT 0
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Volcado de datos para la tabla `canciones`
--

INSERT INTO `canciones` (`id_cancion`, `titulo`, `duracion`, `id_genero`, `idioma`, `id_artista`, `id_album`, `tempoBPM`, `esInstrumental`, `calificacion`, `reproducciones`) VALUES
(1, 'La tierra del olvido', '00:04:25', 1, 'Español', 1, 1, 120, 0, 9.50, 10000),
(2, 'Ojos así', '00:03:57', 3, 'Español', 3, 2, 130, 0, 9.99, 100000),
(3, 'Mi gente', '00:03:05', 4, 'Español', 5, NULL, 105, 0, 9.80, 100000000),
(4, 'Ambiente', '00:04:08', 4, 'Español', 5, 3, 108, 0, 9.99, 234892),
(5, 'Cali pachanguero', '00:04:51', 2, 'Español', 2, 4, 125, 0, 9.99, 54458),
(6, 'La creciente', '00:03:04', 1, 'Español', 4, 5, 110, 0, 9.99, 346789),
(7, 'Sueños de conquista', '00:04:02', 1, 'Español', 4, 6, 115, 0, 9.99, 2568335),
(8, 'Carito', '00:03:39', 3, 'Español', 1, 7, 140, 0, 9.99, 862049),
(9, 'Una aventura', '00:05:16', 2, 'Español', 2, 8, 128, 0, 9.99, 768240),
(10, 'Ginza', '00:04:39', 4, 'Español', 5, NULL, 100, 0, 9.99, 304892),
(11, 'Octavo día', '00:04:32', 3, 'Español', 3, 2, 135, 0, 9.99, 652904),
(12, 'Quiero verte sonreír', '00:03:18', 3, 'Español', 1, 7, 110, 0, 9.99, 16590654),
(13, 'Ginza', '00:04:39', 4, 'Español', 5, NULL, 100, 0, 9.99, 87663);

--
-- Índices para tablas volcadas
--

--
-- Indices de la tabla `canciones`
--
ALTER TABLE `canciones`
  ADD PRIMARY KEY (`id_cancion`),
  ADD KEY `id_genero` (`id_genero`),
  ADD KEY `id_artista` (`id_artista`),
  ADD KEY `id_album` (`id_album`);

--
-- AUTO_INCREMENT de las tablas volcadas
--

--
-- AUTO_INCREMENT de la tabla `canciones`
--
ALTER TABLE `canciones`
  MODIFY `id_cancion` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=14;

--
-- Restricciones para tablas volcadas
--

--
-- Filtros para la tabla `canciones`
--
ALTER TABLE `canciones`
  ADD CONSTRAINT `canciones_ibfk_1` FOREIGN KEY (`id_genero`) REFERENCES `generos` (`id_genero`),
  ADD CONSTRAINT `canciones_ibfk_2` FOREIGN KEY (`id_artista`) REFERENCES `artistas` (`id_artista`),
  ADD CONSTRAINT `canciones_ibfk_3` FOREIGN KEY (`id_album`) REFERENCES `albumes` (`id_album`);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
