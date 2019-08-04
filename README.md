# forca

FIXME: description

## Installation

Download from http://example.com/FIXME.

## Usage

FIXME: explanation

    $ java -jar forca-0.1.0-standalone.jar [args]

## Options

FIXME: listing of options this app accepts.

## Examples

* Instalar o REPL: http://leiningen.org/#install
* Para habilitar a execucao clojure "lein repl".
* Para compilar o clojure: (require '[forca.core :as forca] :reload)
* Executar o projeto: (forca/jogo 3 "CESAR" #{})
* def num [1 2 3] - Declarar uma variavel
* defn mult [ x] (* x 2) - Declarar uma funcao
* defn par [ x] (= 0 (rem x 2)) - Declarar uma funcao utilizando o resto
* map e remove - Funcoes
* (defn numeros [1, 2, 3, 4, 5]) - Cria a array numeros
* (filter (fn [x] (or (< x 2) (> x 4))) numeros) - Filtra todos do conjunto e tira quem nao passa
* (map (fn [x] (* x 3)) numeros) - Roda a funcao para cada numero da array
* (remove (fn [x] (= 1 (rem x 2))) numeros) - Remove numeros impares
* (reduce (fn [a b] (- b a)) numeros ) - Passa a primeira posicao do array no a e passa a segunda posicao do array no b, retorna so 1 valor
* (def palavra #{"A" "L" "U" "R" "O" "E"})
* (filter (fn [x] (or (= x "A") (= x "O"))) palavra) - Verifica se a palavra tem A ou O
* (->> numeros (map (fn [x] (* x 2))) (map (fn [x] (+ x 1))) (reduce (fn [acc next] (+ acc next)))) - Executa varias funciones em sequencia
* Ambos fazem a mesma coisa, porem o segundo e mais legivel:
* (map (fn[x] (- x 200.0)) (map (fn[x] (* x 2.0)) carros))
* (->> carros (map (fn[x] (* x 2))) (map (fn[x] (- x 200))))
* Para rodar o jogo (rodar o main): lein run
* Criar arquivo JAR: lein uberjar
* java -jar forca-0.1.0-SNAPSHOT-standalone.jar
* 

### Bugs

...

### Any Other Sections
### That You Think
### Might be Useful

## License

Copyright © 2019 FIXME

This program and the accompanying materials are made available under the
terms of the Eclipse Public License 2.0 which is available at
http://www.eclipse.org/legal/epl-2.0.

This Source Code may also be made available under the following Secondary
Licenses when the conditions for such availability set forth in the Eclipse
Public License, v. 2.0 are satisfied: GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or (at your
option) any later version, with the GNU Classpath Exception which is available
at https://www.gnu.org/software/classpath/license.html.
