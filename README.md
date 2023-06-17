# lxml_to_dict
conversor lxml a dict

[![PyPI version](https://badge.fury.io/py/nazk.svg)](https://pypi.org/project/nazk/)

## Descripción
Obtén el tipo de cambio oficial de la SBS y SUNAT (Perú) en tiempo real. Nazk es una librería escrita en Python 3.6 que permite obtener de manera rápida y sencilla el tipo de cambio por día o rango de días.

## Instalación
```
pip install lxml_to_dict_total
```

## Uso básico
```python
from lxml_to_dict import lxml_to_dict
 
lxml_to_dict(<the lxml.objectfy.Element>)

root = objectify.Element("root")            # <root></root>
b = objectify.SubElement(root, "b")         # <root><b></b></root>
b = objectify.SubElement(root, "b")         # <root><b></b><b></b></root>
a = objectify.SubElement(root, "a")         # <root><b></b><b></b><a></a></root>
lxml_to_dict(root)                          # {'root': {'b': None, 'b1': None, 'a': None}}
```

## Consideraciones
* Esta es una actualizacion al paquete oficial de `Criva` [https://github.com/CRiva/lxml_to_dict] para uso con python 3.9