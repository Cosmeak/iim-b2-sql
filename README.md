# bdd---sql-guillaume-fine

### Partie 1

SELECT contract.name, COUNT(asset.id) AS nb_contract FROM asset INNER JOIN contract ON asset.contract_id = contract.id GROUP BY contract.id;

SELECT AVG(total_volume) AS Moy_total_volume FROM statistics_general;

SELECT asset.name, order.price FROM `order` INNER JOIN asset ON order.asset_id = asset.id ORDER BY order.price DESC LIMIT 1;

SELECT name, MAX(LENGTH(name)) AS taille FROM contract GROUP BY id ORDER BY taille ASC LIMIT 1;

SELECT contract.name, COUNT(attribute_category.id) AS nb_contract FROM attribute_category INNER JOIN contract ON attribute_category.contract_id = contract.id GROUP BY contract.id;

SELECT contract.name, COUNT(attribute_category.id) AS nb_contract FROM attribute_category INNER JOIN contract ON attribute_category.contract_id = contract.id GROUP BY contract.id ORDER BY nb_contract DESC LIMIT 1;

SELECT contract.name AS contract_name, asset.name AS asset_name FROM asset INNER JOIN contract ON asset.contract_id = contract.id ORDER BY asset.score;

### Partie 2



### Partie 3
