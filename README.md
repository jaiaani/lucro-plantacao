# Lucro de Plantação no Stardew Valley

Minha submissão para o problema 1 da [rinha-de-algoritmo](https://github.com/Universidade-Livre/rinha-de-algoritmos) 2024 da UBL 
(Universidade Brasileira Livre)


![stardew-valley](./resources/stardew-valley.png)


## Usage
🇧🇷
Para executar o programa siga os seguintes passos:

Usando o docker...
 * Nesse mesmo diretório, rode o comando: `docker build -t lucroplantacao .`
 * Depois rode o comando `docker run --rm -it lucroplantacao`
   * Como input há 3 opções: 
      - example1
      - example2
      - example3 
 
   são referentes aos exemplos dados pelo desafio, é somente uma concatenação para se referir
      aos arquivos localizados na pasta ./resources/input,
     ```clojure 
     (defn input
        [example]
        (with-open [rdr (reader (str "./resources/input/" example ".txt"))]
        (doall (mapv vector (line-seq rdr)))))```
   
  se for necessário testar outras entradas, é só adicionar o arquivo nessa pasta.

English -

To run the program, follow these steps:

Using docker...
* In that same directory, run the command: `docker build lucroplantacao .`
* Then run the command `docker run --rm -it lucroplantacao`
    * As input there are 3 options:
        - example1
        - example2
        - example3

  refer to the examples given by the challenge, it is just a concatenation to refer
  to files located in the ./resources/input folder,
    ```clojure 
    (defn input
       [example]
       (with-open [rdr (reader (str "./resources/input/" example ".txt"))]
       (doall (mapv vector (line-seq rdr)))))```

If you need to test other entries, just add the file to this folder.

## Minhas considerações

Só consegui completar o desafio quando encontrei o conceito do problema da mochila,
foi uma explicação que demorou um pouco pra fazer sentido de verdade na minha cabeça,
minha dica é ter paciencia com o processo de aprendizado. Nesse caso eu assisti varios
videos, li uns textos e ainda sim estava confuso. Depois de uma semana quando eu voltei
para o problema as coisas fluiram bem melhor, o processo do entendimento nem sempre é linear
seja paciente e acredite em você :)

Para mais detalhes do problema confere o repositorio da UBL :)
## License

Copyright © 2024 FIXME

This program and the accompanying materials are made available under the
terms of the Eclipse Public License 2.0 which is available at
http://www.eclipse.org/legal/epl-2.0.

This Source Code may also be made available under the following Secondary
Licenses when the conditions for such availability set forth in the Eclipse
Public License, v. 2.0 are satisfied: GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or (at your
option) any later version, with the GNU Classpath Exception which is available
at https://www.gnu.org/software/classpath/license.html.
