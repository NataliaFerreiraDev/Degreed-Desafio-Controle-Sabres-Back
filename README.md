# Degreed-Desafio-Controle-Sabres-Back

<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
</head>

<body>
    <p>Você foi escolhido para ajudar no controle de distribuição de sabres de luz para os novos Jedi.</p>
    <p>Para isso, sua tarefa será desenvolver um sistema para gerenciar o controle dos sabres de luz entregues a cada
        Jedi e seu histórico de manutenção.</p>
    <p>Os sabres de luz podem ser do tipo: Manual, Semiautomático e Automático.</p>
    <p>Todos os sabres de luz possuem algumas informações relevantes que devem ser armazenadas como:</p>
    <table>
        <tr>
            <th>Atributo</th>
            <th>Tipo</th>
            <th>Descrição</th>
            <th>Exemplo</th>
        </tr>
        <tr>
            <td>ID</td>
            <td>Numérico</td>
            <td>Identificador do sabre de luz</td>
            <td>1599</td>
        </tr>
        <tr>
            <td>Modelo</td>
            <td>Texto</td>
            <td>Modelo do sabre de luz na lista de valores: MANUAL, SEMIAUTOMATICO, AUTOMATICO</td>
            <td>MANUAL</td>
        </tr>
        <tr>
            <td>Data de Fabricação</td>
            <td>Data</td>
            <td>Data de fabricação do sabre de luz</td>
            <td>2021-08-10</td>
        </tr>
        <tr>
            <td>Situação</td>
            <td>Texto</td>
            <td>Situação do sabre de luz: PRONTO, OBSOLETO, EM MANUTENÇÂO</td>
            <td>PRONTO</td>
        </tr>
        <tr>
            <td>Histórico de Manutenções</td>
            <td>Mapa</td>
            <td>Histórico de manutenções seguindo a estrutura chave-valor, sendo a chave a data da manutenção e o valor
                o nome do responsável pela manutenção</td>
            <td>"2021-08-11":"Obi-Wan Kenobi"</td>
        </tr>
    </table>
    <p>Os sabres de luz do tipo manual possuem um atributo adicional:</p>
    <table>
        <tr>
            <th>Atributo</th>
            <th>Tipo</th>
            <th>Descrição</th>
            <th>Exemplo</th>
        </tr>
        <tr>
            <td>Modelo Botão Destrava</td>
            <td>Texto</td>
            <td>Modelo do botão de destrava do sabre de luz</td>
            <td>BTN-404</td>
        </tr>
    </table>
    <p>Os sabres de luz do tipo Semiautomático possuem uma manutenção um pouco mais complicada e, portanto, possuem um
        atributo adicional</p>
    <table>
        <tr>
            <th>Atributo</th>
            <th>Tipo</th>
            <th>Descrição</th>
            <th>Exemplo</th>
        </tr>
        <tr>
            <td>Lista de galáxias de Manutenção</td>
            <td>Lista</td>
            <td>Lista de galáxias aptas a realizarem as manutenções</td>
            <td>GN-z11, Via Láctea</td>
        </tr>
    </table>
    <p>Os sabres de luz do tipo Automático possuem mais dois atributos adicionais</p>
    <table>
        <tr>
            <th>Atributo</th>
            <th>Tipo</th>
            <th>Descrição</th>
            <th>Exemplo</th>
        </tr>
        <tr>
            <td>Modelo Sensor Destrava</td>
            <td>Texto</td>
            <td>Modelo do sensor de destrava do sabre de luz</td>
            <td>TX-500</td>
        </tr>
        <tr>
            <td>Data Validade Sensor Destrava</td>
            <td>Data</td>
            <td>Data de validade do sensor de destrava do sabre de luz</td>
            <td>2005-08-10</td>
        </tr>
    </table>
    <p>A entrada das informações deverá ser realizada via console com um número interativo, mas você pode melhorara
        experiência do usuário caso queira utilizar alguma interface gráfica (Java Swing ou JavaFx) e deverá apresentar
        as seguintes opções no menu:</p>
    <ul>
        <li>Cadastrar novo sabre de luz</li>
        <li>Atualizar sabre de luz</li>
        <li>Consultar lista de sabres de luz</li>
        <li>Consultar sabre de luz por ID</li>
    </ul>
    <p>Os dados devem ser persistidos em algum banco de dados de memória de sua preferência por exemplo:</p>
    <ul>
        <li>H2</li>
        <li>HSQLDB</li>
        <li>SQLite</li>
        <li>Derby</li>
    </ul>
    <p>Ao final para ajudar os aliados da resistência a utilizarem seu programa comente os métodos e gere uma
        documentação com o JavaDoc.</p>
    <p>Dicas do Mestre Yoda:</p>
    <ul>
        <li>O atributo ID do sabre de luz é um autoincremento gerado no momento do cadastro</li>
        <li>Avalie se faz sentido utilizar classes abstratas e polimorfismo</li>
        <li>Para valores fixos tente utilizar enums</li>
        <li>Defina os comportamentos em interfaces antes de implementar</li>
        <li>Utilize JDBC para a persistência dos dados com o banco de dados em memória de sua preferência</li>
        <li>Que a força esteja com você</li>
    </ul>
</body>
