# Chatbot para tirar dúvidas dos calouros

Trabalho realizado pelo grupo da disciplina de Inteligencia Artificial.

## Installation

criar uma pasta e criar um ambiente:

```python
$ python3 -m venv ./venv
$ source venv/bin/activate
```

Instalando o aiml:

```bash
$ pip install aiml
```

##### Ao executar o arquivo python e apresentar o erro:

```
Loading /home/kamila/Documentos/chatbot_AIML/conversa.xml...Traceback (most recent call last):
  File "conversa.py", line 4, in <module>
    bot.learn('/home/kamila/Documentos/chatbot_AIML/conversa.xml')
  File "/home/kamila/Documentos/chatbot_AIML/venv/lib/python3.8/site-packages/aiml/Kernel.py", line 335, in learn
    start = time.clock()
AttributeError: module 'time' has no attribute 'clock'

```
##### Podem ser removidos usando os passos:
```
Dentro do venv
abre a pasta chamada lib
Dentro de lib abre a pasta python
Dentro da pasta python abra a pasta Site-packages
Abra a pasta aiml
Abra o arquivo Kernel.py
Aproximadamente na linha 356 vai ter "time.clock()"
Altere para "time.time()"
Existe outra linha nessa mesma função (aproximadamente linha 335) com a mesma expressão "time.clock()"
Altera também Pra "time.time()"

Salve E rode novamente seu programa.
```
