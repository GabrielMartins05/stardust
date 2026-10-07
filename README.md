# Cosmion · A Viagem Diária

Jogo web de trivia de raridade com tema espacial, inspirado no Krillion.io.
Responda cada transmissão com algo **válido, mas o mais raro possível** —
quanto mais rara a resposta, mais anos-luz sua nave avança.

Abra `index.html` direto no navegador: é um arquivo único (HTML + CSS + JS puros), sem build.

| Raridade        | Distância  | Pontos |
|-----------------|-----------:|-------:|
| Poeira Estelar  |    +10 AL  |    +10 |
| Asteroide       |   +100 AL  |    +30 |
| Supernova       |   +300 AL  |    +60 |
| Buraco Negro    |   +600 AL  |   +100 |
| Sem Sinal       |      0 AL  |      0 |

Resposta inválida não pontua nem encerra a transmissão: o jogo avisa e você tenta outra
enquanto houver tempo. Só vira **Sem Sinal** quando o tempo acaba sem resposta válida.

- 7 transmissões por viagem, 20 s cada, sorteadas de um banco de 41 perguntas
  (a viagem diária usa a mesma semente para todos no mesmo dia; "Nova viagem" sorteia outra).
- Respostas são julgadas pelo dicionário `QUESTIONS` no script — ignora acentos,
  maiúsculas, artigos, prefixos ("constelação de…") e pequenos erros de digitação.
- Para adicionar perguntas, inclua um objeto em `QUESTIONS` com as listas de cada nível
  (itens separados por vírgula, sinônimos por `|`).
