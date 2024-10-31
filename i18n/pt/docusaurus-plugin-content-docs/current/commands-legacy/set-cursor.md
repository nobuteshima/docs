---
id: set-cursor
title: SET CURSOR
slug: /commands/set-cursor
displayed_sidebar: docs
---

<!--REF #_command_.SET CURSOR.Syntax-->**SET CURSOR** {( *cursor* )}<!-- END REF-->
<!--REF #_command_.SET CURSOR.Params-->
| Parâmetro | Tipo |  | Descrição |
| --- | --- | --- | --- |
| cursor | Integer | &#8594;  | Número de resource de cursor |

<!-- END REF-->

*Esse comando não é seguro para thread e não pode ser usado em código adequado.*


#### Descrição 

<!--REF #_command_.SET CURSOR.Summary-->O comando SET CURSOR muda o cursor do mouse para o cursos do sistema cujo número de ID você passar em *cursor*.<!-- END REF-->

O comando deve ser chamado no contexto de On Mouse Move [Form event code](form-event-code.md). 

Para restaurar o cursor padrão do mouse, chame o comando sem parâmetros.

Aqui estão os cursores que podem ser passados no parameter *cursor* 

| **Number** | **Cursor**                                    |
| ---------- | --------------------------------------------- |
| 1          | ![](/assets/en/commands/pict14679.en.png)   |
| 2          | ![](/assets/en/commands/pict14680.en.png)   |
| 4          | ![](/assets/en/commands/pict2478657.en.png) |
| 9000       | ![](/assets/en/commands/pict2478660.en.png) |
| 9001       | ![](/assets/en/commands/pict2478662.en.png) |
| 9003       | ![](/assets/en/commands/pict2478664.en.png) |
| 9004       | ![](/assets/en/commands/pict2478666.en.png) |
| 9005       | ![](/assets/en/commands/pict2478669.en.png) |
| 9006       | ![](/assets/en/commands/pict2478671.en.png) |
| 9021       | ![](/assets/en/commands/pict2478674.en.png) |
| 351        | ![](/assets/en/commands/pict2478676.en.png) |
| 9010       | ![](/assets/en/commands/pict2478688.en.png) |
| 9011       | ![](/assets/en/commands/pict2478678.en.png) |
| 9013       | ![](/assets/en/commands/pict2478680.en.png) |
| 9014       | ![](/assets/en/commands/pict2478682.en.png) |
| 9015       | ![](/assets/en/commands/pict2478686.en.png) |
| 9016       | ![](/assets/en/commands/pict2478684.en.png) |
| 9017       | ![](/assets/en/commands/pict2478690.en.png) |
| 9019       | ![](/assets/en/commands/pict2478692.en.png) |
| 9020       | ![](/assets/en/commands/pict2478694.en.png) |
| 559        | ![](/assets/en/commands/pict2478698.en.png) |
| 560        | ![](/assets/en/commands/pict2478696.en.png) |


#### Exemplo 

Se quiser que o cursor seja exibido ![](/assets/en/commands/pict2478692.en.png) quando o mouse mover sobre uma área de variável no formulário. Pode escrever no método de objeto da variável:

```4d
 If(Form event code=On Mouse Move)
    SET CURSOR(9019)
 End if
```
