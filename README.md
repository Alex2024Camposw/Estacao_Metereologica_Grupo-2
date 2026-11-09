>[!Important]
 > `Repositório - Estação Meteorológica`
>- Turma: 2° Semestre de Ciência da Computação.
>- Faculdade: Universidade Paulista.
>- Polo: UNIP Marquês.
>- Sobre: Repositório para a documentação do projeto de Estação Metereológica do 2° Semestre.
>- Membros: Alex Campos de Oliveira, Rafael Arruda, Rafael Alamino, Rafael Torso.

>[!Important]
 > `Referências`
>- `Youtube:` (URL).

> [!NOTE]
 > `Wiki Estruturada:`
>  * [1. ESTAÇÃO METEREOLÓGICA](https://github.com/Alex2024Camposw/Estacao_Metereologica_Grupo-2/wiki/1.-Esta%C3%A7%C3%A3o-Metereol%C3%B3gica)
>  * [2. CODIFICAÇÃO](https://github.com/Alex2024Camposw/Estacao_Metereologica_Grupo-2/wiki/2.-Codifica%C3%A7%C3%A3o)

# 1. ESTAÇÃO METEOROLÓGICA:
#  1.1. Objetivo da Página
 Àrea referente ao projeto da Estação Metereológica, desenvolvida para o 2° semestre de Ciência da Computação. O projeto integra hardware e software, propondo uma solução funcional e completa referente à extração e monitoramento de dados ambientais, junto à filtragem e exclusão de anomalias. Para tal propósito, foi feita uma aplicação com Back-End, Front-End e banco de dados para armazenamento e posteriores consultas de dados metereológicos.
<br> O grupo é composto por:
 * Alex Campos de Oliveira;
 * Rafael Arruda;
 * Rafael Alamino;
 * Rafael Torso.

#  1.2. O Que é o Projeto?
O projeto consiste no desenvolvimento de uma Estação Meteorológica capaz de realizar a coleta, o processamento e o monitoramento de dados ambientais por meio de sensores físicos.
<br>A estrutura integra componentes de hardware, responsáveis pela captação de informações como temperatura, umidade, luminosidade, concentração de gases e pressão atmosférica, a uma aplicação de software responsável pelo recebimento, tratamento e armazenamento dessas informações.
<br>No Back-End, são realizados o processamento dos dados, a aplicação de filtros para identificação e exclusão de possíveis anomalias e a comunicação com o banco de dados MySQL. Já o Front-End disponibiliza uma interface visual para que o usuário possa acompanhar as medições, consultar históricos e visualizar informações da estação meteorológica.
<br>Dessa forma, o projeto busca oferecer uma solução integrada para o monitoramento ambiental, garantindo maior organização, confiabilidade e facilidade de acesso aos dados coletados.

#  1.3. Guia de Instalação e Implementação Web
## 1.3.1. Tecnologias Necessárias
Para o funcionamento e a disponibilização do projeto na Web, são utilizadas diferentes tecnologias que permitem a integração entre o Front-End, Back-End e banco de dados. O desenvolvimento do Back-End utiliza Python e Flask, responsáveis pelo processamento das informações e gerenciamento das requisições HTTP. O Front-End utiliza HTML, CSS e JavaScript para estruturar, estilizar e apresentar os dados meteorológicos ao usuário. Para o armazenamento das informações, é utilizado o MySQL, enquanto o Git e o GitHub são empregados no versionamento e gerenciamento do código-fonte. Em relação à infraestrutura de hospedagem, o Vercel é responsável pela disponibilização do Front-End, o Render pela execução do Back-End e o Aiven pela hospedagem e gerenciamento do banco de dados MySQL.

## 1.3.2. Obtenção do Código-Fonte
Inicialmente, é necessário obter os arquivos do projeto por meio do repositório oficial disponibilizado no GitHub. A plataforma permite acessar, consultar e baixar todos os arquivos necessários para a execução da aplicação. Para realizar esse procedimento, basta acessar o repositório, selecionar a opção de clonagem e executar o comando correspondente no terminal, ou utilizar a opção de download dos arquivos em formato ZIP. Dessa maneira, será possível obter a estrutura completa do projeto, incluindo os arquivos responsáveis pelo Back-End, Front-End e demais configurações.

## 1.3.3. Instalação das Dependências
Após obter o código-fonte, é necessário instalar as dependências utilizadas no desenvolvimento da aplicação. Para isso, deve-se possuir o Python instalado no ambiente de execução e acessar o diretório principal do projeto por meio do terminal. Em seguida, utilizando o arquivo `requirements.txt`, que reúne as bibliotecas necessárias para o funcionamento do Back-End, basta executar o comando `pip install -r requirements.txt`. Esse procedimento realiza a instalação automática dos pacotes utilizados pela aplicação, como Flask, Flask-Cors, NumPy, Requests e demais bibliotecas especificadas no arquivo.

## 1.3.4. Configuração do Ambiente
Com as dependências instaladas, deve-se realizar a configuração das variáveis de ambiente necessárias para a comunicação entre os componentes do sistema. Essas configurações incluem os dados de conexão com o banco de dados MySQL hospedado na plataforma Aiven, além de outras informações utilizadas pelo Back-End. Para isso, deve-se criar e configurar o arquivo `.env`, preenchendo as variáveis com os respectivos valores fornecidos pelos serviços utilizados. É importante garantir que as credenciais de acesso sejam mantidas em segurança, evitando sua exposição no repositório público do GitHub.

## 1.3.5. Execução Local
Após concluir as configurações, a aplicação poderá ser executada localmente para verificar seu funcionamento antes da implantação definitiva na Web. Para iniciar o Back-End, deve-se acessar o diretório principal do projeto e executar o comando `python -m js.Main_Back` no terminal. Com o servidor iniciado, será possível realizar requisições à aplicação e verificar a comunicação com o banco de dados, além de testar o recebimento, processamento e disponibilização das informações meteorológicas. O Front-End poderá ser acessado localmente por meio de um servidor HTTP, permitindo validar a interface e suas funcionalidades.

## 1.3.6. Implantação e Hospedagem Web
A disponibilização do projeto na Internet é realizada por meio da integração de três plataformas distintas. O Front-End é hospedado no Vercel, responsável por disponibilizar os arquivos HTML, CSS e JavaScript e permitir o acesso à interface por meio de uma URL pública. O Back-End é implantado no Render, que executa a aplicação Python utilizando o servidor Gunicorn, responsável por atender às requisições recebidas e processar os dados meteorológicos. Já o banco de dados MySQL é hospedado na plataforma Aiven, que oferece a infraestrutura necessária para armazenar, organizar e disponibilizar os registros utilizados pela aplicação. Durante a implantação, é necessário configurar corretamente as variáveis de ambiente, os endereços de comunicação e as permissões de acesso entre os serviços, garantindo a integração adequada entre os três componentes.

## 1.3.7. Acesso à Aplicação
Após a conclusão da implantação e a configuração dos serviços, a aplicação estará disponível para acesso pela Internet, por meio do endereço público fornecido pelo Vercel. O usuário poderá acessar o sistema diretamente pelo navegador, sem precisar instalar ou executar manualmente os componentes do projeto. A interface permitirá acompanhar as informações coletadas pela Estação Meteorológica, visualizar os dados processados pelo Back-End e consultar os registros armazenados no banco de dados MySQL hospedado na Aiven.

#  1.4. Esquemas Eletrônicos
## 1.4.1. Esquema Eletrônico
| <p align = "center">  Imagem - Esquema Eletrônico do Protótipo Físico Final </p> | 
|---|
| <img width="100%" height="80%" alt="image" src="https://github.com/user-attachments/assets/2568c63b-0380-4f42-9154-4d5c602067f9"/>|
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |


#  1.5. Fotos do Protótipo

## 1.5.1. Protótipo Físico Final
| <p align = "center">  Imagem - Protótipo Físico Final </p> | 
|---|
| <img width="100%" height="80%" alt="pf" src="https://github.com/user-attachments/assets/33afca8d-1fbc-4ff5-b5fe-7e88d0179a66" />|
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

## 1.5.2. Protótipo Físico I
| <p align = "center">  Imagem - Protótipo Físico I </p> | 
|---|
| <img width="100%" height="80%" alt="image" src="https://github.com/user-attachments/assets/7bf32f68-1efe-4e15-afe3-584d7cdae32b"/> |
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

## 1.5.3. Protótipo Físico II
| <p align = "center">  Imagem - Protótipo Físico II </p> | 
|---|
| <img width="100%" height="80%" alt="image" src="https://github.com/user-attachments/assets/eb07876f-17ce-4c83-9811-8d2abdb0c1f8" /> |
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

#  1.6. Demonstrações da Interface

## 1.6.1. Interface I
| <p align = "center">  Interface I </p> | 
|---|
| <img width="854" height="480" alt="ITF I" src="https://github.com/user-attachments/assets/376c22d6-128e-4ad9-94e8-c6fc7b83da57"/> |
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

## 1.6.2. Interface II
| <p align = "center">  Interface II </p> | 
|---|
| <img width="854" height="480" alt="ITF 2" src="https://github.com/user-attachments/assets/70304d9e-a31e-4f86-8702-ca03200dd8ce" /> |
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

## 1.6.3. Interface III
| <p align = "center">  Interface III </p> | 
|---|
| <img width="854" height="480" alt="ITF 3" src="https://github.com/user-attachments/assets/61e00d33-614e-48c0-a67f-26d25019d6a8" /> |
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

## 1.6.4. Interface IV
| <p align = "center">  Interface IV </p> | 
|---|
|<img width="854" height="480" alt="ITF 4" src="https://github.com/user-attachments/assets/6d610c4b-d1c0-4217-a6ec-4a98dc81f912" />|
| <p align = "center"> Fonte: Grupo 2, 2026. </p> |

# 2. CODIFICAÇÃO:
<details>
<summary> <strong>HTML</strong> </summary>
<details>
<summary> Index.HTML </summary>
 
 ```csharp
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
    <link rel="stylesheet" href="css/style.css">
    <title>Dashboard-Unip</title>
</head>
<body>
    <div class="conteiner">
        <aside>
            <div class="top">
               <div class="logo">
                    <img src="img/unip-163.png" alt="">
                    <h2>UNIP <span class="badge">PRO</span></h2>
                </div>
                <div class="close" id="close-btn">
                    <span class="material-symbols-outlined">close</span>
                </div>
            </div>
            <div class="sidebar">
                <a href="index.html">
                    <span class="material-symbols-outlined">grid_view</span>
                    <h3>Dashboard</h3>
                </a>
                 <a href="ingestao.html">
                   <span class="material-symbols-outlined">tune</span>
                    <h3>Ingestão de Dados</h3>
                </a>
                 <a href="analises.html">
                    <span class="material-symbols-outlined">bar_chart</span>
                    <h3>Análises</h3>
                </a>
                 <a href="configuracoes.html">
                    <span class="material-symbols-outlined">settings</span>
                    <h3>Configurações</h3>
                </a>
                 <a href="mapa.html">
                  <span class="material-symbols-outlined">map</span>
                    <h3>Mapa</h3>
                </a>
                 <a href="logout.html">
                  <span class="material-symbols-outlined">logout</span>
                    <h3>Logout</h3>
                </a>
            </div>
        </aside>
        <!----------------------End aside------------------>
        <main>
            <h1>Dashboard</h1>
            <div class="date">
                <input id ="Date_Filter" type="date">
            </div>
            <div class="insights">
                <div class="temperature">
                    <span class="material-symbols-outlined">thermostat</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Temp.Média</h3>
                            <h1 id = "temperatura"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_temperatura"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End temperatura------------------------------>
                 <div class="humidity">
                    <span class="material-symbols-outlined">water_drops</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Umidade Média</h3>
                            <h1 id = "umidade"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_umidade"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End humidity------------------------------>
                 <div class="windspeed">
                   <span class="material-symbols-outlined">speed</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Pressão</h3>
                            <h1 id = "pressão"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_pressão"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End vento------------------------------>
                <!-----------------------End humidity------------------------------>
                 <div class="luz">
                    <span class="material-symbols-outlined">light_mode</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Luminosidade</h3>
                            <h1 id = "luminosidade"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_luminosidade"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End vento------------------------------>
                <!-----------------------End humidity------------------------------>
                 <div class="Gás">
                  <span class="material-symbols-outlined">co2</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Gás</h3>
                            <h1 id = "gás"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_gas"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End gas------------------------------>
            </div>
            <!--------------------------END INSIGHTS----------------------------->
            <div class="recent-orders">
                <h2>Processamento de Dados de campo</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Estação (Nome)</th>
                            <th>Estação (ID)</th>
                            <th>Último Recebimento</th>
                        </tr>
                    </thead>
                    <tbody>
                    </tbody>
                </table>
                <a href="#">Ver tudo</a>
            </div>
        </main>
        <!---------------------END OF MAIN-------------->
        <div class="right">
            <div class="top">
                <button id="menu-btn">
                    <span class="material-symbols-outlined">menu</span>
                </button>
                <div class="theme-toggler">
                    <span class="material-symbols-outlined active">light_mode</span>
                    <span class="material-symbols-outlined">dark_mode</span>
                </div>
                <div class="profile">
                    <div class="info">
                        <p>Hey, <b>Tester</b></p>
                      
                    </div>
                    <div class="profile-photo">
                        <img src="img/profile-33.png" alt="">
                    </div>
                </div>
            </div>
            <!--end top-------->
            <div class="recent-updates">
                <h2>Recebimento Recente</h2>
                <div class="updates">
                    <div class="update">
                        <div class="profile-photo">
                            <img src="img/ESTAÇÃO.png" alt="">
                        </div>
                        <div class="message">
                            <b> <p id = "Recent_Station_Name"> </p></b>
                            <p id = "Recent_Station_Data"></p>
                            <small id = "Recent_Station_Time" class="text-muted"></small>
                        </div>
                    </div>
                    </div>
                </div>
            <!----------------END RECENT UPDATES---------------------------->
             <div class="Systems-analytics">
                <h2>Análise do Sistema</h2>
                <div class="item online">
                    <div class="icon">
                        <span class="material-symbols-outlined">language</span>
                    </div>
                    <div class="right">
                        <div class="info">
                            <b> <p id = "Analytics_Station_Name"> </p> </b>
                            <small class="text-muted" id = "Analytics_Time"> </small>
                        </div>
                        <h3 class="success" id = "Analytics_Updates_Value"> </h3>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </div>
</div>
    <script src="js/Dashboard.js"></script>
    
</body>
</html>
```
</details>

<details>
<summary> analises.html </summary>

 ```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Análises - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Análises Climáticas</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="content-card">
                <h3>Exportar Relatórios</h3>
                <p>Selecione um período para baixar os dados tratados da rede de sensoriamento.</p>
                <div class="form-group-inline">
                    <input type="date" id="Date_Filter_Report">
                    <button class="btn-primary" id="btnRelatorio">Gerar Relatório CSV</button>
                </div>
            </div>
             <!-- Indicadores em Tempo Real -->
            <div class="content-card">
                <h3>Indicadores em Tempo Real (Gauges)</h3>
                <div class="insights" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem; margin-top: 1rem;">
                    <div class="card">
                        <div class="middle">
                            <div class="left">
                                <h3>Temperatura</h3>
                                <h1 id="temperatura">--</h1>
                            </div>
                        </div>
                        <small class="text-muted" id="%_temperatura">--</small>
                    </div>

                    <div class="card">
                        <div class="middle">
                            <div class="left">
                                <h3>Umidade</h3>
                                <h1 id="umidade">--</h1>
                            </div>
                        </div>
                        <small class="text-muted" id="%_umidade">--</small>
                    </div>

                    <div class="card">
                        <div class="middle">
                            <div class="left">
                                <h3>Pressão do Ar</h3>
                                <h1 id="pressão">--</h1>
                            </div>
                        </div>
                        <small class="text-muted" id="%_pressão">--</small>
                    </div>

                    <div class="card">
                        <div class="middle">
                            <div class="left">
                                <h3>Luminosidade</h3>
                                <h1 id="luminosidade">--</h1>
                            </div>
                        </div>
                        <small class="text-muted" id="%_luminosidade">--</small>
                    </div>
                </div>
            </div>

            <!-- Gráfico Histórico -->
<div class="content-card" style="margin-top: 2rem;">
    <h3>Gráficos Históricos da Estação</h3>
    <div id="containerGraficos" class="graficos-grid">
        <div class="grafico-card">
            <h4>Temperatura</h4>
            <div class="grafico-area">
                <canvas id="graficoHistorico_temperatura"></canvas>
            </div>
        </div>

        <div class="grafico-card">
            <h4>Umidade</h4>
            <div class="grafico-area">
                <canvas id="graficoHistorico_umidade"></canvas>
            </div>
        </div>

        <div class="grafico-card">
            <h4>Pressão atmosférica</h4>
            <div class="grafico-area">
                <canvas id="graficoHistorico_pressão"></canvas>
            </div>
        </div>

        <div class="grafico-card">
            <h4>Qualidade do ar (gás)</h4>
            <div class="grafico-area">
                <canvas id="graficoHistorico_gás"></canvas>
            </div>
        </div>
    </div>
</div>
            <!-- Histórico de Registros -->
            <div class="content-card recent-orders" style="margin-top: 2rem;">
                <h3>Histórico de Registros</h3>
                <table>
                    <thead>
                        <tr>
                            <th>Estação</th>
                            <th>ID da Estação</th>
                            <th>Data e Hora</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td colspan="3">Carregando histórico...</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </main>
    </div>
    <script src="js/Dashboard.js"></script>
</body>
</html>
```

</details>

<details>
<summary> configuracoes.html </summary>

```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Configurações - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Configurações do Sistema</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="content-card">
                <h2>Preferências Gerais</h2>
                <form class="settings-form">
                    <div class="field">
                        <label>Unidade de Temperatura:</label>
                        <select>
                            <option>Celsius (°C)</option>
                            <option>Fahrenheit (°F)</option>
                        </select>
                    </div>
                    <div class="field checkbox-field">
                        <input type="checkbox" id="notif" checked>
                        <label for="notif">Receber notificações por E-mail</label>
                    </div>
                    <button type="button" class="btn-primary">Salvar Alterações</button>
                </form>
            </div>
        </main>
    </div>
    <script src="js/Preferencias.js"></script>
</body>
</html>
```


</details>

<details>
<summary> ingestao.html </summary>

```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ingestão De Dados - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Ingestão De Dados</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="table-card">
                <h2>Log de Transmissão de Pacotes em Tempo Real</h2>
                <div class="table-responsive">
                    <table>
                        <thead>
                            <tr>
                                <th>Origem</th>
                                <th>Protocolo</th>
                                <th>Tamanho</th>
                                <th>Status</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </main>
    </div>
    <script src="js/Dashboard.js"></script>
</body>
</html>
```


</details>


<details>
<summary> mapa.html </summary>

```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mapa Interativo - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
    
    <!-- CSS do Leaflet -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Mapa Interativo das Estações</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="map-card">
                <div id="map" style="width: 100%; height: 500px;"></div>
            </div>
        </main>
    </div>
    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
    <script src="js/Mapa.js"></script>
</body>
</html>
```
</details>
</details>

<details>
<summary> <strong>CSS</strong>  </summary>
<details>
<summary> style.css </summary>

```csharp
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    margin: 0;
    padding: 0;
    outline: none;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
}

:root {
    --black: #000000; 
    --red: #0468fd;
    --white: #FFFFFF;
    --gray: #867e7e;
    --color-primary: #7380ec;
    --color-danger: #ff7782;
    --color-success: #41f1b6;
    --color-warning: #ffbb55;
    --color-white: #fff;
    --color-info-dark: #7d8da1;
    --color-info-light: #dce1eb;
    --color-dark: #363949;
    --color-light: rgba(132, 139, 200, 0.18);
    --color-primary-variant: #111e88;
    --color-dark-variant: #677483;
    --color-background: #f6f6f9;

    --card-border-radius: 2rem;
    --border-radius-1: 0.4rem;
    --border-radius-2: 0.8rem;
    --border-radius-3: 1.2rem;

    --card-padding: 1.8rem;
    --padding-1: 1.2rem;

    --box-shadow: 0 2rem 3rem var(--color-light);
}

/* ---------- DARK THEME VARIABLES ---------- */
.dark-theme-variables {
    --color-background: #181a1e;
    --color-white: #202528;
    --color-dark: #edeffd;
    --color-dark-variant: #a3bdcc;
    --color-light: rgba(0, 0, 0, 0.4);
    --box-shadow: 0 2rem 3rem var(--color-light);
}

body {
    font-family: "Poppins", sans-serif;
    width: 100vw;
    min-height: 100vh;
    overflow-x: hidden;
    background-color: var(--color-background);
    user-select: none;
    color: var(--color-dark);
}


a { color: var(--color-dark); }
img { display: block; width: 100%; }

h1 { font-weight: 800; font-size: 1.8rem; }
h2 { font-size: 1.4rem; }
h3 { font-size: 0.87rem; }
h4 { font-size: 0.8rem; }
h5 { font-size: 0.77rem; }
small { font-size: 0.75rem; }

.text-muted { color: var(--color-info-dark); }
p { color: var(--color-dark-variant); }
b { color: var(--color-dark); }

.primary { color: var(--color-primary); }
.danger { color: var(--color-danger); }
.success { color: var(--color-success); }
.warning { color: var(--color-primary); }

/* ================= TELA DE LOGIN & REGISTRO ================= */
.login-background {
    background-image: url('img/fundo.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    width: 100vw;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
}

.conteiner2 {
    position: relative;
    width: 420px;
    max-width: 100%;
    height: 500px;
    background-color: transparent;
    border: 2px solid var(--red);
    border-radius: 10px;
    color: var(--red);
    padding: 30px 40px;
    box-shadow: 0 0 10px rgba(0, 0, 0, .2);
    backdrop-filter: blur(5px);
    overflow: hidden;
    transition: height .4s ease, border-color 0.5s ease;
}

.conteiner2.active {
    height: 580px;
}

.conteiner2 h1 {
    font-size: 36px;
    text-align: center;
}

.input-box {
    position: relative;
    width: 100%;
    height: 50px;
    margin: 20px 0;
}

.input-box input {
    width: 100%;
    height: 100%;
    background-color: transparent;
    border: 1px solid var(--black); 
    border-radius: 40px;
    outline: none;
    font-size: 16px;
    color: #FFFFFF;
    padding: 0 45px 0 20px; 
}

.input-box input::placeholder {
    color: var(--gray);
}

.input-box i {
    position: absolute;
    right: 20px;
    font-size: 20px;
    top: 50%;
    transform: translateY(-50%);
}

.remember-forgot {
    display: flex;
    justify-content: space-between;
    font-size: 14px;
    margin: -5px 0 15px;
}

.remember-forgot label input {
    accent-color: var(--white);
    margin-right: 5px;
}

.remember-forgot a {
    color: var(--gray);
}

.remember-forgot a:hover {
    text-decoration: underline;
}

.Loginbutton {
    width: 100%;
    height: 50px;
    background-color: var(--red);
    border: none;
    border-radius: 40px;
    cursor: pointer;
    font-size: 16px;
    color: var(--white);
    font-weight: 600;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
    margin-top: 10px;
    transition: 0.3s;
}

.Loginbutton:hover {
    background-color: transparent;
    border: 2px solid rgba(255, 255, 255, .2);
    color: var(--black);
}

.register-link {
    font-size: 14px;
    text-align: center;
    margin: 20px 0 15px;
}

.register-link a {
    color: var(--gray);
    font-weight: 600;
}

.register-link a:hover {
    text-decoration: underline;
}

.conteiner2:hover {
    border-color: var(--white);
    animation: border-glow 1s infinite alternate;
}

@keyframes border-glow {
    from {
        border-color: var(--red);
        box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }
    to {
        border-color: var(--red);
        box-shadow: 0 0 20px rgba(255, 255, 255, .1);
    }
}

.form-box {
    width: 100%;
    transition: transform .5s ease;
}

.conteiner2 .form-box.login {
    transform: translateX(0);
}

.conteiner2.active .form-box.login {
    transform: translateX(-500px);
}

.conteiner2 .form-box.register {
    position: absolute;
    top: 30px;
    left: 40px;
    right: 40px;
    width: calc(100% - 80px);
    transform: translateX(500px);
}

.conteiner2.active .form-box.register {
    transform: translateX(0);
}

.form-box.register .icon-close {
    position: absolute;
    top: -10px;
    left: -15px;
    width: 35px;
    height: 35px;
    background: var(--red);
    font-size: 1.6em;
    color: var(--white);
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    cursor: pointer;
    z-index: 10;
    transition: background 0.3s ease, transform 0.2s ease;
}

.form-box.register .icon-close:hover {
    background: var(--black);
    transform: scale(1.1);
}

/* ================= DASHBOARD LAYOUT ================= */
.conteiner {
    display: grid;
    width: 96%;
    margin: 0 auto;
    gap: 1.8rem;
    grid-template-columns: 14rem auto 23rem;
}

/* ---------- SIDEBAR ---------- */
aside {
    height: 100vh;
}

aside .top {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 1.4rem;
}

aside .logo {
    display: flex;
    gap: 0.8rem;
}

aside .logo img {
    width: 6rem;
    height: 6rem;
}

aside .close {
    display: none;
}

aside .logo h2 {
    display: flex;
    align-items: center;
    gap: 0.5rem;
}

aside .logo .badge {
    background: var(--color-primary, #7380ec);
    color: #fff;
    font-size: 0.65rem;
    padding: 0.2rem 0.5rem;
    border-radius: 0.4rem;
    font-weight: 600;
    text-transform: uppercase;
}

aside .sidebar {
    display: flex;
    flex-direction: column;
    height: calc(100vh - 6rem);
    position: relative;
    top: 3rem;
}

aside h3 {
    font-weight: 500;
}

aside .sidebar a {
    display: flex;
    color: var(--color-info-dark);
    margin-left: 2rem;
    gap: 1.2rem;
    align-items: center;
    position: relative;
    height: 4rem;
    transition: all 300ms ease;
}

aside .sidebar a span {
    font-size: 1.8rem;
    transition: all 300ms ease;
}

aside .sidebar a h3 {
    font-size: 1rem;
    font-weight: 500;
}

aside .sidebar a:last-child {
    position: absolute;
    bottom: 1rem;
    width: 100%;
}

aside .sidebar a.active {
    background: var(--color-light);
    color: var(--color-primary);
    margin-left: 0;
}

aside .sidebar a.active::before {
    content: "";
    width: 8px;
    height: 100%;
    background: var(--color-primary, #7380ec);
    position: absolute;
    left: 0;
    top: 0;
    border-radius: 0 4px 4px 0;
}

aside .sidebar a.active span {
    color: var(--color-primary);
    margin-left: calc(1rem - 3px);
}

aside .sidebar a:hover {
    color: var(--color-primary);
}

aside .sidebar a:hover span {
    margin-left: 1rem;
}

/* ---------- MAIN CONTENT & BOTÃO VOLTAR ---------- */
main {
    margin-top: 1.4rem;
}

.page-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.8rem;
    flex-wrap: wrap;
    gap: 1rem;
}

.btn-back {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: var(--color-primary);
    color: var(--color-white);
    padding: 0.6rem 1.2rem;
    border-radius: var(--border-radius-1);
    font-weight: 500;
    transition: all 300ms ease;
}

.btn-back:hover {
    opacity: 0.85;
    transform: translateX(-3px);
}

main .date {
    display: inline-block;
    background: var(--color-light);
    border-radius: var(--border-radius-1);
    margin-top: 1rem;
    padding: 0.3rem 1rem;
    box-shadow: 0 0.5rem 1rem var(--color-light);
}

main .date input[type='date'] {
    background: transparent;
    color: var(--color-dark);
    border: none;
    outline: none;
    font-family: inherit;
    font-size: 0.9rem;
    cursor: pointer;
}

.date input[type="date"]::-webkit-calendar-picker-indicator {
    cursor: pointer;
    filter: invert(0.4);
}

main .insights {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.6rem;
}

main .insights > div {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    margin-top: 1rem;
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

main .insights > div:hover {
    box-shadow: none;
}

main .insights > div span {
    background: red;
    padding: 0.5rem;
    border-radius: 50%;
    color: var(--color-white);
    font-size: 2rem;
}

main .insights > div.humidity span {
    background: var(--red);
}

main .insights > div.windspeed span {
    background: var(--color-warning);
}

main .insights > div.luz span {
    background: #eeff55; /* Fundo Amarelo do Ícone */
}

main .insights > div.Gás span {
    background: #867e7e; /* Fundo Cinza do Ícone */
}

main .insights > div .middle {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

main .insights > div .left {
    margin-right: 0.1rem;
}

main .insights h3 {
    margin: 1rem 0 0.6rem;
    font-size: 1rem;
}

main .insights .progress {
    position: relative;
    width: 92px;
    height: 92px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

main .insights svg {
    width: 92px;
    height: 92px;
    transform: rotate(-90deg);
}

main .insights svg circle {
    fill: none;
    stroke-width: 10;
    stroke-linecap: round;
    transform: translate(8px, 8px);
}

main .insights .temperature svg circle {
    stroke: #ff5252;
    filter: drop-shadow(0px 3px 6px rgba(255, 82, 82, 0.4));
    stroke-dashoffset: -30;
    stroke-dasharray: 200;
}

main .insights .humidity svg circle {
    stroke: #0468fd;
    filter: drop-shadow(0px 3px 6px rgba(4, 104, 253, 0.45));
    stroke-dashoffset: 20;
    stroke-dasharray: 80;
}

main .insights .windspeed svg circle {
   stroke: #ff7700; /* Círculo de Progresso Laranja */
    filter: drop-shadow(0px 3px 6px rgba(255, 119, 0, 0.45));
    stroke-dashoffset: 45;
    stroke-dasharray: 90;
}

main .insights .luz svg circle {
    stroke: #fffc3a; /* Círculo de Progresso Amarelo */
    filter: drop-shadow(0px 3px 6px rgba(255, 187, 85, 0.45));
    stroke-dashoffset: 45;
    stroke-dasharray: 90;
}

main .insights .Gás svg circle {
    stroke: #867e7e; /* Círculo de Progresso Cinza */
    filter: drop-shadow(0px 3px 6px rgba(134, 126, 126, 0.45));
    stroke-dashoffset: 45;
    stroke-dasharray: 90;
}

main .insights .progress .number {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    padding: 0;
}

main .insights .progress .number p {
    font-weight: 600;
    font-size: 0.85rem;
    line-height: 1;
}

main .insights small {
    margin-top: 1.3rem;
    display: block;
}

/* ---------- TABELAS / RECENT ORDERS ---------- */
main .recent-orders {
    margin-top: 2rem;
    overflow-x: auto;
}

main .recent-orders h2 {
    margin-bottom: 0.8rem;
}

main .recent-orders table {
    background: var(--color-white);
    width: 100%;
    border-radius: var(--card-border-radius);
    padding: var(--card-padding);
    text-align: center;
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

main .recent-orders table:hover {
    box-shadow: none;
}

main table tbody td {
    height: 2.8rem;
    border-bottom: 1px solid var(--color-light);
    color: var(--color-dark-variant);
}

main table tbody tr:last-child td {
    border: none;
}

main .recent-orders a {
    text-align: center;
    display: block;
    margin: 1rem auto;
    color: var(--color-primary);
}

/* ---------- DIREITA / RIGHT PANEL ---------- */
.right {
    margin-top: 1.4rem;
}

.right .top {
    display: flex;
    justify-content: end;
    gap: 2rem;
}

.right .top button {
    display: none;
}

.right .theme-toggler {
    background: var(--color-light);
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 1.6rem;
    width: 4.2rem;
    cursor: pointer;
    border-radius: var(--border-radius-1);
}

.right .theme-toggler span {
    font-size: 1.2rem;
    width: 50%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.right .profile {
    display: flex;
    gap: 1rem;
    align-items: center;
    text-align: right;
}

.right .profile .info p {
    margin: 0;
    font-size: 0.9rem;
}

.right .profile .info small {
    display: block;
    margin-top: -2px;
}

.right .profile-photo {
    width: 2.8rem;
    height: 2.8rem;
    border-radius: 50%;
    overflow: hidden;
}

.right .profile-photo img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transform: scale(6.2);
}

.right .theme-toggler span.active {
    background: var(--color-primary);
    color: white;
    border-radius: var(--border-radius-1);
}

.right .recent-updates {
    margin-top: 1rem;
}

.right .recent-updates h2 {
    margin-bottom: 0.8rem;
}

.right .recent-updates .updates {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

.right .recent-updates .updates:hover {
    box-shadow: none;
}

.right .recent-updates .updates .update {
    display: grid;
    grid-template-columns: 2.6rem auto;
    gap: 1rem;
    margin-top: 1rem;
}

.right .Systems-analytics {
    margin-top: 2rem;
}

.right .Systems-analytics h2 {
    margin-bottom: 0.8rem;
}

.right .Systems-analytics .item {
    background: var(--color-white);
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 0.7rem;
    padding: 1.4rem var(--card-padding);
    border-radius: var(--border-radius-3);
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

.right .Systems-analytics .item:hover {
    box-shadow: none;
}

.right .Systems-analytics .item .right {
    display: flex;
    justify-content: space-between;
    align-items: start;
    margin: 0;
    width: 100%;
}

.right .Systems-analytics .item .icon {
    padding: 0.6rem;
    color: var(--color-white);
    border-radius: 50%;
    background: var(--color-primary);
    display: flex;
}

.right .Systems-analytics .item.offline .icon {
    background: var(--color-danger);
}

.right .Systems-analytics .item.customers .icon {
    background: var(--color-success);
}

/* ================= ESTRUTURAS DAS PÁGINAS SECUNDÁRIAS ================= */

/* Layout sem Sidebar */
.container-single {
    width: 92%;
    max-width: 1200px;
    margin: 2rem auto;
    display: block;
}

/* Cards de Conteúdo Gerais */
.content-card, 
.table-card, 
.map-card,
.form-container, 
.form-card {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    margin-top: 1rem;
    width: 100%;
}

/* Mapa Interativo (Leaflet/Google Maps) */
#map {
    width: 100%;
    height: 520px;
    border-radius: var(--border-radius-2);
    z-index: 1;
}

/* Tabelas Responsivas para Subpáginas */
.table-responsive,
.table-container {
    width: 100%;
    overflow-x: auto;
    margin-top: 1rem;
}

.table-responsive table,
.table-container table {
    width: 100%;
    border-collapse: collapse;
    text-align: left;
}

.table-responsive th, .table-responsive td,
.table-container th, .table-container td {
    padding: 1rem;
    border-bottom: 1px solid var(--color-light);
}

.table-responsive th, .table-container th {
    color: var(--color-info-dark);
    font-weight: 600;
}

.badge-status {
    padding: 0.3rem 0.8rem;
    border-radius: var(--border-radius-1);
    font-size: 0.8rem;
    font-weight: 600;
}

.badge-status.success { background: rgba(65, 241, 182, 0.2); color: #0d9467; }
.badge-status.danger { background: rgba(255, 119, 130, 0.2); color: #d32f2f; }

/* Formulários das Páginas Secundárias */
.form-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.2rem;
    margin-bottom: 1.5rem;
}

.form-group {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.form-group input, 
.form-group select, 
.form-group textarea,
.settings-form select, 
.settings-form input[type="date"] {
    width: 100%;
    padding: 0.8rem 1rem;
    border-radius: var(--border-radius-1);
    border: 1px solid var(--color-info-light);
    background: var(--color-background);
    color: var(--color-dark);
    font-family: inherit;
    font-size: 0.9rem;
}

.form-actions {
    display: flex;
    gap: 1rem;
    justify-content: flex-end;
    flex-wrap: wrap;
}

.btn-primary {
    padding: 0.8rem 1.5rem;
    background: var(--color-primary);
    color: var(--color-white);
    border: none;
    border-radius: var(--border-radius-1);
    cursor: pointer;
    font-weight: 600;
    transition: opacity 300ms ease;
}

.btn-primary:hover {
    opacity: 0.9;
}

/* Grids de Cards / Analytics */
.cards-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.6rem;
    margin-top: 1rem;
}

.card-item {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

.card-item:hover {
    box-shadow: none;
}

.chart-container {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    margin-top: 1rem;
    position: relative;
    width: 100%;
    min-height: 320px;
}

/* ================= MEDIA QUERIES (RESPONSIVIDADE COMPLETA) ================= */

/* Login - Celulares */
@media (max-width: 480px) {
    .conteiner2 {
        padding: 25px 20px;
    }

    .conteiner2 .form-box.register {
        left: 20px;
        right: 20px;
        width: calc(100% - 40px);
    }

    .conteiner2 h1 {
        font-size: 28px;
    }

    .remember-forgot {
        font-size: 12px;
        flex-direction: column;
        gap: 8px;
    }

    .form-box.register .icon-close {
        left: -5px;
        top: -15px;
    }

    .form-actions {
        flex-direction: column;
    }

    .form-actions button, 
    .form-actions a {
        width: 100%;
        text-align: center;
    }
}

/* Dashboard & Layout - Notebooks / Tablets Grandes */
@media screen and (max-width: 1200px) {
    .conteiner {
        width: 94%;
        grid-template-columns: 7rem auto 23rem;
    }

    aside .logo h2,
    aside .sidebar h3 {
        display: none;
    }

    aside .sidebar a {
        width: 5.6rem;
    }

    aside .sidebar a:last-child {
        position: relative;
        margin-top: 1.8rem;
    }

    main .insights {
        grid-template-columns: 1fr;
        gap: 0;
    }

    main .recent-orders {
        width: 94%;
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        margin: 2rem 0 0 8.8rem;
    }

    main .recent-orders table {
        width: 83vw;
    }

    main table thead tr th:first-child,
    main table tbody tr td:first-child,
    main table thead tr th:last-child,
    main table tbody tr td:last-child {
        display: none;
    }
}

/* Dashboard & Páginas Secundárias - Celulares e Tablets */
@media screen and (max-width: 768px) {
    .conteiner {
        width: 100%;
        grid-template-columns: 1fr;
        padding-top: 4rem;
    }

    .container-single {
        width: 95%;
        padding: 0 0.5rem;
        margin-top: 1rem;
    }

    aside {
        position: fixed;
        left: -100%;
        background: var(--color-white);
        width: 18rem;
        z-index: 10;
        box-shadow: 1rem 3rem 4rem var(--color-light);
        height: 100vh;
        padding-right: var(--card-padding);
        display: none;
        animation: showMenu 400ms ease forwards;
    }
    
    aside .sidebar a:last-child {
        position: relative; /* Mudado de absolute para relative no mobile */
        bottom: 0;
        margin-top: 2rem;
        margin-bottom: 2rem;
    }


    @keyframes showMenu {
        to {
            left: 0;
        }
    }

    aside .logo {
        margin-left: 1rem;
    }
    
    aside .logo h2,
    aside .sidebar h3 {
        display: inline;
    }

    aside .sidebar a {
        width: 100%;
        height: 3.4rem;
    }

    aside .sidebar a:last-child {
        position: absolute;
        bottom: 5rem;
    }

    aside .close {
        display: inline-block;
        cursor: pointer;
    }

    main {
        margin-top: 1rem;
        padding: 0 1rem;
    }

    .page-header {
        flex-direction: column;
        align-items: flex-start;
    }

    .btn-back {
        width: 100%;
        justify-content: center;
    }

    #map {
        height: 380px;
    }

    main .recent-orders {
        position: relative;
        margin: 2rem 0 0 0;
        width: 100%;
        overflow-x: auto;
    }

    main .recent-orders table {
        width: 100%;
        margin: 0;
    }

    main table thead tr th:first-child,
    main table tbody tr td:first-child,
    main table thead tr th:last-child,
    main table tbody tr td:last-child {
        display: none;
    }

    .right {
        width: 100%;
        margin: 0 auto 4rem;
        padding: 0 1rem;
    }

    .right .top {
        position: fixed;
        top: 0;
        left: 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 1.5rem;
        height: 4.6rem;
        background: var(--color-white);
        width: 100%;
        margin: 0;
        z-index: 5;
        box-shadow: 0 0.5rem 1rem var(--color-light);
    }

    .right .top button {
        display: flex;
        align-items: center;
        justify-content: center;
        background: transparent;
        border: none;
        cursor: pointer;
        color: var(--color-dark);
        position: static;
    }

    .right .top button span {
        font-size: 2rem;
    }

    .right .top .theme-toggler {
        width: 4.4rem;
        position: static;
    }

    .right .profile .info {
        display: none;
    }

    .form-grid,
    .cards-grid {
        grid-template-columns: 1fr;
    }
}
/* ==========================================================================
   ESTILOS DO MAPA INTERATIVO (LEAFLET)
   ========================================================================== */
#map {
    width: 100%;
    height: 500px;
    border-radius: 1rem;
    z-index: 1;
}

.map-card {
    width: 100%;
    min-height: 500px;
}

/* ==========================================
   ESTILOS PARA ALERTAS FLUTUANTES (TOASTS)
   ========================================== */
.toast-container {
    position: fixed;
    bottom: 20px;
    right: 20px;
    z-index: 9999;
    display: flex;
    flex-direction: column;
    gap: 10px;
    pointer-events: none;
}

.toast {
    pointer-events: auto;
    min-width: 280px;
    padding: 12px 16px;
    background: var(--color-white);
    color: var(--color-dark);
    border-left: 5px solid #41f1b6;
    border-radius: var(--border-radius-1);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 0.85rem;
    animation: slideInRight 0.3s ease, fadeOut 0.5s ease 4.5s forwards;
}

.toast .toast-content {
    display: flex;
    align-items: center;
    gap: 10px;
}

.toast .toast-icon {
    color: #0d9467;
    font-size: 1.3rem;
}

.toast .toast-close {
    cursor: pointer;
    color: var(--color-info-dark);
    font-size: 1.1rem;
    background: none;
    border: none;
}

@keyframes slideInRight {
    from { transform: translateX(100%); opacity: 0; }
    to { transform: translateX(0); opacity: 1; }
}

@keyframes fadeOut {
    from { opacity: 1; }
    to { opacity: 0; transform: translateY(-10px); }
}

/* ==========================================
   ESTILOS PARA ALERTAS IN-LINE (BADGES)
   ========================================== */
.badge-inline {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    padding: 2px 8px;
    border-radius: 12px;
    font-size: 0.72rem;
    font-weight: 600;
    margin-left: 6px;
    text-transform: uppercase;
}

.badge-inline.ok {
    background-color: rgba(65, 241, 182, 0.2);
    color: #0d9467;
}

.badge-inline.alerta {
    background-color: rgba(255, 119, 130, 0.2);
    color: #d32f2f;
}
```

</details>


</details>

<details>
<summary> <strong>SQL</strong>  </summary>

<details>
<summary> Estacao_Metereologica.sql </summary>
 
```csharp
create database Estacao_Meteorologica;
use Estacao_Meteorologica;

SET SQL_SAFE_UPDATES = 0;

create table tbEstacao(
Id_Estacao int (10) primary key,
Nome_Estacao char (100) not null,
latitude float (4,2),
longitude float (4,2)	
);

create table tbLeitura(
 Id_Leitura BigInt primary key auto_increment,
 Id_Estacao int (10) not null,
 temperatura float (4,2),
 qualidade_ar int,
 luminosidade int,
 umidade float (4,2),
 pressao float (4,2),
 data_hora timestamp,

 foreign key (Id_Estacao) references tbEstacao(Id_Estacao)
);

-- Alterando as tabelas para o modelo requisitado pelo documento, apagando valores nulos e os substituindo por um valor padrão de "0".
alter table tbLeitura modify column temperatura float(4,2) not null default 0;
alter table tbLeitura modify column qualidade_ar int not null default 0;
alter table tbLeitura modify column  luminosidade int not null default 0;
alter table tbLeitura modify column umidade float(4,2) not null default 0;
alter table tbLeitura modify column pressao float(4,2) not null default 0;
alter table tbLeitura modify column data_hora timestamp not null;
describe tbLeitura;

-- Alterando as colunas da tbEstacao para que não aceitem valores nulos. Também alterando o tipo de dado para que seja mais condizente com o que é requisitado.
alter table tbEstacao modify column latitude point not null;
alter table tbEstacao modify column longitude point not null;
describe tbEstacao;
```
</details>
<details>
<summary> Select.sql </summary>
 
```csharp
select * from tbEstacao;
select * from tbLeitura;
select * from tbLeitura where data_hora = '2026-10-01'/
```
</details>
</details>

<details>
<summary> <strong>Back-End</strong>  </summary>
 <details>
<summary> Main_Back.py </summary>
  
```csharp

# Importa a classe responsável por armazenar e atualizar os dados dos sensores.
from js.Back_End.Dados import Dado

# Importa a função responsável por filtrar os dados históricos.
from js.Back_End.Filtragem import Filtrar_Dados

# Importa funções para verificar e padronizar datas.
from js.Back_End.Data import Verificar_Data, Formatar_para_Padrao

# Importa funções responsáveis pela comunicação com o banco de dados.
from js.Back_End.Banco import (
    Inserir_Dados_no_Banco,
    Puxar_Data,
    Puxar_Id,
    Puxar_Historico,
    Puxar_Nome_Estacao
)

# Importa a classe responsável por consultar a API meteorológica.
from js.Back_End.HTTP import API

# Importa a classe responsável pelo gerenciamento de alertas.
from js.Back_End.Alertas import Alerta

# Importa os recursos necessários para criar e gerenciar a aplicação Flask.
from flask import Flask, request, jsonify
from flask_cors import CORS

# Importa bibliotecas para carregar variáveis de ambiente,
# controlar o tempo, executar tarefas em paralelo e realizar cálculos.
from dotenv import load_dotenv
import os
import time
import threading
import math
import numpy as np


# Lista utilizada para armazenar valores identificados como exceções pelo filtro MMS.
Lista_Excecoes = []


# Função responsável por corrigir valores que não podem ser convertidos para JSON.
# Valores como NaN e infinito são substituídos por zero.
def Corrigir_Valor_JSON(valor):
    if isinstance(valor, float) and not math.isfinite(valor):
        return 0
    return valor


# Função responsável por aplicar o filtro de Média Móvel Simples (MMS).
# Tipo_Dado representa o sensor que terá seus valores filtrados.
# Intervalo define a quantidade de valores utilizados no cálculo da média.
# Tolerancia define a diferença máxima permitida entre o valor atual e a média.
def Filtro_MMS(Tipo_Dado, Intervalo=100, Tolerancia=100):
    global Lista_Excecoes, OBJ_Alerta

    print("No filtro MMS.")

    # Percorre todos os valores recebidos pelo sensor.
    for Valor in Tipo_Dado.Campo_Valor:

        # Converte o valor atual para o tipo float.
        valor_atual = float(Valor)

        # Verifica se já existem dados suficientes para calcular a média móvel.
        if len(Tipo_Dado.Campo_Filtrado) >= Intervalo:

            # Seleciona os últimos valores aceitos pelo filtro.
            ultimos_dados = Tipo_Dado.Campo_Filtrado[-Intervalo:]

            # Calcula a média dos valores selecionados.
            mms_atual = sum(ultimos_dados) / Intervalo

            # Verifica se a diferença entre o valor atual e a média ultrapassa a tolerância.
            if abs(valor_atual - mms_atual) > Tolerancia:

                # Registra o valor considerado uma exceção.
                Lista_Excecoes.append({
                    "Campo": Tipo_Dado.Campo_Tipo,
                    "Excecao": valor_atual,
                    "Mms_esperada": mms_atual
                })

                # Ignora o valor atual e continua a análise dos próximos dados.
                continue

        # Se o valor estiver dentro da tolerância, ele é aceito pelo filtro.
        Tipo_Dado.Campo_Filtrado.append(valor_atual)


# Carrega as variáveis de ambiente armazenadas no arquivo .env.
load_dotenv()

# Cria a aplicação Flask.
app = Flask(__name__)

# Define os endereços autorizados a realizar requisições ao backend.
Origens_Permitidas = [
    "http://127.0.0.1:5500",
    "http://localhost:5500",
    "https://projetos-estacao-meteorol-gica-grupo-3de5.vercel.app"
]

# Configura o CORS utilizando a lista de origens permitidas.
CORS(app, origins=Origens_Permitidas)

# Obtém a porta de execução disponibilizada pelo servidor.
# Caso não exista uma variável PORT, utiliza a porta 3000.
PORT = int(os.getenv("PORT", 3000))


# Realiza a primeira consulta à API meteorológica.
# A resposta é armazenada em dados_API e seu código HTTP em Status_Code.
dados_API, Status_Code = API.Buscar_Dados_HTTP(True)

# Exibe os dados recebidos no terminal.
print(dados_API)


# Lista utilizada para armazenar os dados gerais da estação.
Lista_de_Dados = []

# Lista responsável por armazenar os alertas meteorológicos.
Lista_Alerta = []

# Instancia a classe de alertas, passando a lista que receberá os alertas.
OBJ_Alerta = Alerta(Lista_Alerta)


# Inicializa as referências dos sensores.
# Os objetos serão criados após uma consulta bem-sucedida à API.
Temperatura = None
Umidade = None
Luminosidade = None
Gas = None
Pressao = None


# Armazena a quantidade de campos atualizados durante uma leitura.
Qtd_Campos_Atualizados = 0

# Recupera o histórico de leituras armazenado no banco de dados.
Historico_de_Dados = Puxar_Historico()

# Inicializa listas utilizadas para armazenar valores das leituras e da estação.
Valores_Leitura = []
Valores_Estacao = []


# Obtém o identificador do último registro disponível na API.
API_ID_Anterior = dados_API["channel"]["last_entry_id"]
API_Novo_ID = dados_API["channel"]["last_entry_id"]

# Indica se os dados da estação foram atualizados.
Dados_Atualizados = False


# Recupera o identificador da estação meteorológica no banco de dados.
Id_Estacao = Puxar_Id("tbEstacao")

# Obtém as informações de identificação e localização da estação pela API.
Nome_Estacao = dados_API["channel"]["name"]
latitude = dados_API["channel"]["latitude"]
longitude = dados_API["channel"]["longitude"]

# Inicializa as variáveis responsáveis pelo controle de data e horário.
Data_Hora_Atual = None
Data_Hora_Anterior = Puxar_Data()


# Verifica se a estação já está cadastrada no banco de dados.
if Id_Estacao is None:

    # Caso não exista, utiliza o identificador fornecido pela API.
    Id_Estacao = dados_API["channel"]["id"]

    # Organiza as informações necessárias para cadastrar a estação.
    Valores_Estacao = [
        Id_Estacao,
        Nome_Estacao,
        latitude,
        longitude
    ]

    # Insere os dados da estação na tabela correspondente.
    Inserir_Dados_no_Banco(
        Valores_Estacao,
        "tbEstacao"
    )

else:
    # Informa que a estação já possui cadastro.
    print("Estacao ja existe.")


# Função responsável por atualizar os objetos dos sensores
# e realizar o processamento dos dados recebidos.
def Atualizar_Objetos():

    print(">>> ATUALIZAR OBJETOS EXECUTADA <<<")

    # Permite modificar as variáveis globais da aplicação.
    global Qtd_Campos_Atualizados, Dados_Atualizados

    # Atualiza os valores de cada sensor utilizando os dados recebidos da API.
    Temperatura.Atualizar_Dados(dados_API["feeds"])
    Umidade.Atualizar_Dados(dados_API["feeds"])
    Luminosidade.Atualizar_Dados(dados_API["feeds"])
    Gas.Atualizar_Dados(dados_API["feeds"])
    Pressao.Atualizar_Dados(dados_API["feeds"])

    # Aplica o filtro MMS aos sensores.
    # Cada sensor possui um intervalo e uma tolerância específicos.
    Filtro_MMS(Temperatura, Intervalo=50, Tolerancia=10)
    Filtro_MMS(Umidade, Intervalo=50, Tolerancia=10)
    Filtro_MMS(Luminosidade, Intervalo=50, Tolerancia=150)
    Filtro_MMS(Gas, Intervalo=50, Tolerancia=50)
    Filtro_MMS(Pressao, Intervalo=50, Tolerancia=5)

    # Verifica se os valores filtrados ultrapassam os limites estabelecidos.
    # Caso ultrapassem, a classe de alertas poderá registrar um alerta.
    OBJ_Alerta.Procurar_Alerta(
        "Temperatura", 10, float(Temperatura.Campo_Filtrado[-1])
    )
    OBJ_Alerta.Procurar_Alerta(
        "Umidade", 10, float(Umidade.Campo_Filtrado[-1])
    )
    OBJ_Alerta.Procurar_Alerta(
        "Luminosidade", 150, float(Luminosidade.Campo_Filtrado[-1])
    )
    OBJ_Alerta.Procurar_Alerta(
        "Gas", 50, float(Gas.Campo_Filtrado[-1])
    )
    OBJ_Alerta.Procurar_Alerta(
        "Pressao", 5, float(Pressao.Campo_Filtrado[-1])
    )

    # Indica que o processo de atualização foi concluído.
    Dados_Atualizados = True

    # Registra a quantidade de campos atualizados.
    Qtd_Campos_Atualizados = Dado.Qtd_Atualizado

    # Zera o contador para a próxima atualização.
    Dado.Zerar_Contabilizador()


# Função responsável por organizar os valores que serão armazenados no banco.
def Montar_Valores_Banco():

    # Retorna os dados da estação na ordem esperada pela tabela tbLeitura.
    return [
        Id_Estacao,
        Temperatura.Campo_Filtrado[-1],
        Gas.Campo_Filtrado[-1],
        Luminosidade.Campo_Filtrado[-1],
        Umidade.Campo_Filtrado[-1],
        Pressao.Campo_Filtrado[-1],
        Data_Hora_Atual
    ]


# Função responsável por inserir uma nova leitura no banco de dados
# e atualizar o histórico disponibilizado pela aplicação.
def Atualizar_Banco():

    # Permite atualizar as variáveis globais utilizadas pela aplicação.
    global Valores_Leitura
    global Historico_de_Dados
    global Nome_Estacao

    # Organiza os valores da leitura atual.
    Valores_Leitura = Montar_Valores_Banco()

    # Insere a leitura na tabela tbLeitura.
    Inserir_Dados_no_Banco(Valores_Leitura, "tbLeitura")

    # Recupera novamente o histórico após a inserção.
    Historico_de_Dados = Puxar_Historico()

    # Atualiza o nome da estação utilizando o banco de dados.
    Nome_Estacao = Puxar_Nome_Estacao()


# Inicializa os objetos dos sensores caso a primeira requisição HTTP tenha sido bem-sucedida.
if Status_Code == 200:

    Temperatura = Dado("field1", dados_API["feeds"])
    Umidade = Dado("field2", dados_API["feeds"])
    Luminosidade = Dado("field3", dados_API["feeds"])
    Gas = Dado("field6", dados_API["feeds"])
    Pressao = Dado("field7", dados_API["feeds"])


# Função principal responsável por consultar periodicamente a API
# e atualizar os dados da estação meteorológica.
def Main():

    # Declara as variáveis globais que serão modificadas dentro da função.
    global dados_API
    global Status_Code
    global API_Novo_ID
    global API_ID_Anterior
    global Data_Hora_Atual
    global Data_Hora_Anterior
    global Dados_Atualizados

    print(">>> FUNÇÃO MAIN INICIADA <<<")

    # Inicia o ciclo contínuo de atualização.
    while True:

        # Aguarda cinco segundos antes de realizar uma nova consulta.
        time.sleep(5)

        # Atualiza os objetos dos sensores com os dados disponíveis.
        Atualizar_Objetos()

        print(">>> CONSULTANDO API <<<")

        # Consulta novamente a API meteorológica.
        dados_API, Status_Code = API.Buscar_Dados_HTTP(True)

        # Verifica se a consulta foi realizada com sucesso.
        if Status_Code != 200:
            print("Erro ao consultar a API:", Status_Code)
            continue

        # Obtém o identificador do registro mais recente.
        API_Novo_ID = dados_API["channel"]["last_entry_id"]

        # Compara o identificador atual com o último identificador registrado.
        # Se forem iguais, significa que não existe uma nova leitura.
        if API_Novo_ID == API_ID_Anterior:
            print("Nenhuma atualizacao.")
            continue

        # Obtém e padroniza a data e o horário da última leitura.
        Data_Hora_Atual = Formatar_para_Padrao(
            dados_API["feeds"][-1]["created_at"]
        )

        print("Data-Hora:", Data_Hora_Atual)

        # Verifica se a leitura já foi registrada anteriormente.
        if Verificar_Data(Data_Hora_Anterior, Data_Hora_Atual):

            print("Dado repetido")
            print("Historico Obtido:", Historico_de_Dados)
            continue

        else:
            # Identifica a chegada de uma nova leitura.
            print("Novo dado encontrado")

            # Atualiza o identificador e a data de referência.
            API_ID_Anterior = API_Novo_ID
            Data_Hora_Anterior = Data_Hora_Atual

            # Processa os novos valores dos sensores.
            Atualizar_Objetos()

            # Armazena os dados processados no banco de dados.
            Atualizar_Banco()

            print("Estado da Atualizacao:", Dados_Atualizados)
            print("ID Novo:", API_Novo_ID)
            print("ID Anterior:", API_ID_Anterior)


# Rota responsável por disponibilizar os dados da estação ao frontend.
@app.route("/dados", methods=["GET"])
def Obter_Dados():

    # Permite alterar a variável global após enviar a resposta.
    global Dados_Atualizados

    # Verifica se foi solicitada uma consulta histórica por data.
    if request.args.get("data"):
        return Filtrar_Dados()

    # Monta um dicionário contendo os dados que serão enviados em JSON.
    resposta = {

        # Identificação da estação meteorológica.
        "Nome_Estacao": Nome_Estacao,

        # Valores atuais dos sensores.
        "temperatura": Corrigir_Valor_JSON(Temperatura.Campo_Filtrado[-1]),
        "umidade": Corrigir_Valor_JSON(Umidade.Campo_Valor[-1]),
        "luminosidade": Corrigir_Valor_JSON(Luminosidade.Campo_Valor[-1]),
        "gás": Corrigir_Valor_JSON(Gas.Campo_Valor[-1]),
        "pressão": Corrigir_Valor_JSON(Pressao.Campo_Valor[-1]),

        # Informações sobre a atualização e o histórico de leituras.
        "Qtd_Atualizados": Qtd_Campos_Atualizados,
        "Historico_de_Dados": Historico_de_Dados,
        "Data_Hora": Data_Hora_Atual,
        "Atualizacao": Dados_Atualizados,
        "Codigo_HTTP": Status_Code,

        # Coordenadas geográficas da estação.
        "latitude": latitude,
        "longitude": longitude,

        # Lista de alertas e indicador de existência de alertas.
        "alerta": Lista_Alerta,
        "estado_alerta": OBJ_Alerta.TemAlerta
    }

    # Reseta a indicação de atualização após preparar a resposta.
    Dados_Atualizados = False

    # Converte o dicionário em uma resposta JSON para o frontend.
    return jsonify(resposta)


# Cria uma thread independente para executar o ciclo de atualização.
# O daemon permite que a thread seja encerrada junto com o processo principal.
# Fica fora do bloco __main__ para funcionar quando a aplicação é iniciada pelo Gunicorn.
threading.Thread(
    target=Main,
    daemon=True
).start()


# Executa o servidor Flask diretamente quando o arquivo é iniciado como programa principal.
# No Render, o Gunicorn importa o objeto app e assume a inicialização do servidor.
if __name__ == "__main__":

    app.run(
        host="0.0.0.0",
        port=PORT,
        debug=False,
        use_reloader=False
    )
```

</details>
<details>
<summary> Banco.py </summary>

```csharp
# Importa a biblioteca responsável por acessar variáveis e recursos do sistema operacional.
import os

# Importa a biblioteca utilizada para conectar e executar comandos no MySQL.
import mysql.connector

# Importa a função responsável por carregar as variáveis de ambiente do arquivo .env.
from dotenv import load_dotenv

# Importa recursos para trabalhar com datas e horários.
from datetime import datetime


# Carrega as variáveis de ambiente armazenadas no arquivo .env.
load_dotenv()


# Cria a conexão com o banco de dados MySQL utilizando as informações do arquivo .env.
conexao = mysql.connector.connect(
    host=os.getenv("DB_host"),
    port=os.getenv("DB_port"),
    user=os.getenv("DB_user"),
    password=os.getenv("DB_password"),
    database=os.getenv("DB_database")
)


# As funções abaixo realizam consultas (SELECT) e inserções (INSERT) no banco de dados.


# Busca o nome da estação meteorológica cadastrada no banco.
def Puxar_Nome_Estacao():

    # Cria um cursor que retorna os resultados das consultas em formato de dicionário.
    cursor = conexao.cursor(dictionary=True)

    try:
        # Define o comando SQL para buscar o nome da estação.
        Select_Nome_Estacao = """
            SELECT Nome_Estacao
            FROM tbEstacao;
        """

        # Executa o comando SQL no banco de dados.
        cursor.execute(Select_Nome_Estacao)

        # Recupera todos os registros encontrados.
        resultado = cursor.fetchall()

        # Exibe o resultado da consulta no console.
        print("Estação:", resultado)

        # Verifica se algum registro foi encontrado.
        if resultado:
            return resultado[0]["Nome_Estacao"]

        # Caso não encontre registros, retorna None.
        return None

    # Captura erros relacionados ao MySQL.
    except mysql.connector.Error as erro:
        print("Erro ao buscar estação:", erro)
        raise

    # Fecha o cursor independentemente do resultado da operação.
    finally:
        cursor.close()


# Busca todos os registros de leituras armazenados no histórico.
def Puxar_Historico():

    # Cria um cursor que retorna os resultados em formato de dicionário.
    cursor = conexao.cursor(dictionary=True)

    try:
        # Define o comando SQL para buscar todas as informações das leituras.
        Historico_Select = """
            SELECT Id_Estacao, temperatura, qualidade_ar,
                   luminosidade, umidade, pressao, data_hora
            FROM tbLeitura;
        """

        # Executa a consulta no banco de dados.
        cursor.execute(Historico_Select)

        # Recupera todos os registros encontrados.
        resultado = cursor.fetchall()

        # Exibe o histórico recebido no console.
        print("Histórico Puxado no Banco:", resultado)

        # Retorna a lista com todos os registros encontrados.
        return resultado

    except mysql.connector.Error as erro:
        print("Erro ao puxar histórico:", erro)
        raise

    finally:
        # Fecha o cursor após finalizar a consulta.
        cursor.close()


# Busca as leituras meteorológicas correspondentes a uma data específica.
def Pegar_Dados_Filtrados(Data_do_Filtro):

    # Cria um cursor para executar comandos SQL e receber resultados em dicionários.
    cursor = conexao.cursor(dictionary=True)

    try:
        # Verifica se alguma data foi recebida.
        # Caso contrário, retorna uma lista vazia.
        if not Data_do_Filtro:
            return []

        # Tenta converter a data recebida para o formato de data do Python.
        try:
            Data_Formatada = datetime.strptime(Data_do_Filtro, "%Y-%m-%d").date()

        # Caso a data esteja em um formato inválido, gera um erro.
        except (ValueError, TypeError):
            raise ValueError(f"Data inválida recebida no filtro: {Data_do_Filtro}")

        # Define o comando SQL para buscar as leituras do dia selecionado.
        # DATE_ADD adiciona um dia à data para estabelecer o limite final da consulta.
        Select_Dados = """
            SELECT Id_Estacao, temperatura, qualidade_ar,
                   luminosidade, umidade, pressao, data_hora
            FROM tbLeitura
            WHERE data_hora >= %s
              AND data_hora < DATE_ADD(%s, INTERVAL 1 DAY)
            ORDER BY data_hora ASC;
        """

        # Executa a consulta utilizando a data recebida como parâmetro.
        cursor.execute(
            Select_Dados,
            (Data_Formatada, Data_Formatada)
        )

        # Recupera todos os registros correspondentes à data selecionada.
        resultado = cursor.fetchall()

        # Exibe a data filtrada e a quantidade de registros encontrados.
        print(
            f"Filtro: {Data_Formatada} | "
            f"Registros encontrados: {len(resultado)}"
        )

        # Retorna os registros encontrados.
        return resultado

    # Captura erros que possam ocorrer durante a consulta.
    except Exception as erro:
        print("ERRO AO BUSCAR DADOS FILTRADOS:", repr(erro))
        raise

    finally:
        # Fecha o cursor após finalizar a operação.
        cursor.close()


# Busca a data e o horário da leitura mais recente registrada no banco.
def Puxar_Data():

    # Cria um cursor que retorna os resultados em formato de dicionário.
    cursor = conexao.cursor(dictionary=True)

    try:
        # Define o comando SQL para buscar a leitura mais recente.
        Data_Select = """
            SELECT data_hora
            FROM tbLeitura
            ORDER BY data_hora DESC
            LIMIT 1;
        """

        # Executa a consulta no banco.
        cursor.execute(Data_Select)

        # Recupera somente o primeiro registro encontrado.
        resultado = cursor.fetchone()

        # Verifica se não existem leituras cadastradas.
        if resultado is None:
            print("Nenhuma leitura encontrada.")
            return None

        # Obtém a data e o horário do registro encontrado.
        Data = resultado["data_hora"]

        # Converte a data para texto.
        Data_Formatada = str(Data)

        # Exibe a data obtida no console.
        print("Resultado Retornado:", Data_Formatada)

        # Retorna a data formatada.
        return Data_Formatada

    except mysql.connector.Error as erro:
        print("Erro ao buscar data:", erro)
        raise

    finally:
        # Fecha o cursor após finalizar a consulta.
        cursor.close()


# Busca o primeiro ID existente na tabela informada.
def Puxar_Id(Tabela):

    # Cria um cursor para executar a consulta e receber resultados em dicionários.
    cursor = conexao.cursor(dictionary=True)

    try:
        # Verifica qual tabela foi informada e define sua respectiva coluna de ID.
        if Tabela == "tbLeitura":
            Coluna_Id = "Id_Leitura"

        elif Tabela == "tbEstacao":
            Coluna_Id = "Id_Estacao"

        # Caso a tabela não seja reconhecida, gera um erro.
        else:
            raise ValueError("Tabela inválida.")

        # Monta o comando SQL para buscar o menor ID da tabela.
        Id_Tabela = f"""
            SELECT {Coluna_Id}
            FROM {Tabela}
            ORDER BY {Coluna_Id}
            LIMIT 1;
        """

        # Executa a consulta no banco de dados.
        cursor.execute(Id_Tabela)

        # Recupera o primeiro registro encontrado.
        resultado = cursor.fetchone()

        # Caso não existam registros, retorna None.
        if resultado is None:
            return None

        # Retorna o valor do ID encontrado.
        return resultado[Coluna_Id]

    except mysql.connector.Error as erro:
        print("Erro ao buscar ID:", erro)
        raise

    finally:
        # Fecha o cursor após finalizar a consulta.
        cursor.close()


# Insere novos dados na tabela informada do banco de dados.
def Inserir_Dados_no_Banco(Dados_Leitura, Tabela):

    # Cria um cursor para executar comandos SQL.
    cursor = conexao.cursor()

    try:
        # Verifica se os dados serão inseridos na tabela de estações.
        if Tabela == "tbEstacao":

            # Define o comando SQL para inserir os dados da estação.
            Leitura = """
                INSERT INTO tbEstacao
                (Id_Estacao, Nome_Estacao, Latitude, Longitude)
                VALUES (%s, %s, %s, %s);
            """

        # Verifica se os dados serão inseridos na tabela de leituras.
        elif Tabela == "tbLeitura":

            # Define o comando SQL para inserir os dados meteorológicos.
            Leitura = """
                INSERT INTO tbLeitura
                (Id_Estacao, temperatura, qualidade_ar,
                 luminosidade, umidade, pressao, data_hora)
                VALUES (%s, %s, %s, %s, %s, %s, %s);
            """

        # Caso a tabela informada não seja reconhecida, gera um erro.
        else:
            raise ValueError("Tabela inválida.")

        # Executa o comando SQL utilizando os dados recebidos como parâmetros.
        cursor.execute(Leitura, Dados_Leitura)

        # Confirma a inserção dos dados no banco de dados.
        conexao.commit()

        # Exibe o ID gerado pelo banco após a inserção.
        print("Dados inseridos no Banco:", cursor.lastrowid)

        # Retorna o ID do registro inserido.
        return cursor.lastrowid

    # Caso ocorra algum erro durante a inserção, executa o tratamento abaixo.
    except Exception as erro:

        # Desfaz as alterações realizadas na transação.
        conexao.rollback()

        # Exibe o erro ocorrido durante a inserção.
        print("Erro ao inserir:", erro)

        # Repassa o erro para que possa ser tratado em outra parte do programa.
        raise

    finally:
        # Fecha o cursor após finalizar a operação.
        cursor.close()


# Verifica se a conexão com o banco de dados está ativa.
if conexao.is_connected():
    print("Conectado ao MySQL!")

# Encerra a conexão com o banco de dados quando necessário.
def Fechar_Conexao():

    # Verifica se a conexão ainda está ativa antes de fechá-la.
    if conexao.is_connected():

        # Encerra a conexão com o MySQL.
        conexao.close()
        # Exibe uma mensagem confirmando o encerramento.
        print("Conexão com MySQL encerrada.")
```

</details>
<details>
<summary> Dados.py </summary>

```csharp
# Cria a classe responsável por armazenar e organizar os dados meteorológicos.
class Dado:

    # Atributo de classe que contabiliza a quantidade de registros atualizados.
    Qtd_Atualizado = 0

    # Inicializa a classe recebendo o tipo de dado e a referência dos dados.
    def __init__(self, Campo_Tipo, Ref_Dados):
        # Armazena o tipo de informação que será trabalhada.
        self.Campo_Tipo = Campo_Tipo
        # Cria uma lista para armazenar as datas dos registros.
        self.Campo_Data = []
        # Cria uma lista para armazenar os valores numéricos dos registros.
        self.Campo_Valor = []
        # Cria uma lista para armazenar os dados após algum processo de filtragem.
        self.Campo_Filtrado = []
        # Adiciona os dados recebidos às listas correspondentes.
        self.Adicionar_Dados(Ref_Dados)


    # Percorre os dados recebidos e separa seus valores e datas.
    def Adicionar_Dados(self, Ref_Dado):
        # Percorre cada registro recebido.
        for Dados in Ref_Dado:
            try:
                # Tenta converter o valor do registro para o formato float.
                Valor_Float = float(Dados[self.Campo_Tipo])
            # Caso a conversão falhe, atribui NaN (valor numérico inválido).
            except (ValueError, TypeError):
                Valor_Float = float("nan")

            # Armazena o valor convertido na lista de valores.
            self.Campo_Valor.append(Valor_Float)
            # Armazena a data correspondente ao registro.
            self.Campo_Data.append(Dados["created_at"])


    # Atualiza os dados armazenados com uma nova lista de registros.
    def Atualizar_Dados(self, Ref_Dados):

        # Limpa os valores antigos antes de inserir os novos registros.
        self.Campo_Valor = []
        self.Campo_Data = []
        # Zera o contador de registros atualizados.
        Dado.Zerar_Contabilizador()

        # Percorre os novos registros recebidos.
        for Dados in Ref_Dados:
            try:
                # Tenta converter o valor do registro para float.
                Valor_Float = float(Dados[self.Campo_Tipo])
            # Caso a conversão falhe, atribui NaN.
            except (ValueError, TypeError):
                Valor_Float = float("nan")

            # Adiciona o valor convertido à lista de valores.
            self.Campo_Valor.append(Valor_Float)
            # Adiciona a data correspondente à lista de datas.
            self.Campo_Data.append(Dados["created_at"])
            # Incrementa o contador de registros processados.
            Dado.Contabilizar_Campos_Registrados()


    # Método estático responsável por incrementar o contador de registros.
    # Pode ser utilizado diretamente pela classe, sem criar um objeto.
    @staticmethod
    def Contabilizar_Campos_Registrados():
        # Incrementa a quantidade de registros atualizados.
        Dado.Qtd_Atualizado += 1
        # Retorna a quantidade atualizada.
        return Dado.Qtd_Atualizado


    # Método estático responsável por zerar o contador de registros.
    @staticmethod
    def Zerar_Contabilizador():
        # Reinicia o contador de registros.
        Dado.Qtd_Atualizado = 0
        # Retorna o contador após ser zerado.
        return Dado.Qtd_Atualizado
```

</details>
<details>
<summary> Data.py </summary>

```csharp
def Verificar_Data(Data_Anterior, Data_Atual):
    print(f"{Data_Atual} : {Data_Anterior}")

    if Data_Atual == Data_Anterior:
        print("Datas Iguais. Interrompido")
        return True
    else:
        print("Datas diferentes. Dar seguimento")
        return False


def Formatar_para_MYSQL(Data_Normal):
    if not Data_Normal:
        return None

    return f"{Data_Normal} 00:00:00"


def Formatar_para_Padrao(data):
    if not data:
        return None

    return data.replace("T", " ").replace("Z", "")
```

</details>
<details>
<summary> Filtragem.py </summary>

```csharp
from flask import request, jsonify
from js.Back_End.Banco import Pegar_Dados_Filtrados

def Filtrar_Dados():
    Data_para_Filtrar = request.args.get("data")

    try:
        Dados_Filtrados = Pegar_Dados_Filtrados(Data_para_Filtrar)

        print("DADOS:", Dados_Filtrados)

        return jsonify(Dados_Filtrados)

    except Exception as erro:
        print("Erro ao filtrar:", erro)

        return jsonify({
            "erro": "Erro ao buscar dados filtrados"
        }), 500

```

</details>
<details>
<summary> HTTP.py </summary>

```csharp
import os
import requests
from dotenv import load_dotenv
load_dotenv()

class HTTP:
    def __init__(self, URL):
        self.URL = URL
        
    def Buscar_Dados_HTTP(self, Pegar_HTTP=False):
        resposta = requests.get(self.URL)
        dados = resposta.json()

        if Pegar_HTTP is True:
            HTTP_Status = resposta.status_code
            return dados, HTTP_Status

        return None

    def Buscar_Dados(self):
        resposta = requests.get(self.URL)
        dados = resposta.json()
        return dados
    
API = HTTP(os.getenv("API_URL"))
```

</details>
</details>

<details>
<summary> <strong>Front-End</strong>  </summary>
<details>
<summary> Dashboard.js </summary>

```csharp
// Variável global utilizada para armazenar os dados da atualização padrão.
let dados;

// Lista que armazena os registros recém chegados do Back-End para apresentar no formato de um histórico de registros.
let Registro_do_Historico = [];

// Variável global para controle do estado de filtragem. Se verdadeiro, pausa a atualização padrão da aplicação por um período maior.
let Pausar_Atualização = false;

// Contador utilizado para determinar qual registro será inserido no Dashboard.
let Contador_Registros;

//
let Ultimo_Dado;

// URL que possui a rota em que os dados do Back-End são enviados.
const RENDER_URL = "https://projetos-estacao-meteorol-gica.onrender.com/dados";

// Identifica o elemento de filtrar da página "Index" e da página de "Análise".
const Filtro_de_Data = document.getElementById("Date_Filter") ?? document.getElementById("Date_Filter_Report")

// Lista que receberá os gráficos de cada tipo de dado posteriormente.
const Graficos = {};

// Controle para identificar se formulário de filtrar por data existe para depois aplicar o evento.
if (Filtro_de_Data) {
    Filtro_de_Data.addEventListener("change", Filtrar_por_Data);
} else {
    console.log("Botão de filtrar não encontrado");
}

// Função auxiliar para retornar os dados ao Back-End. Recebe a informação e uma String para criar o caminho (url).
async function Retornar_Dados_ao_Back(Dado_a_Retornar, Local_STR) {
    try {
        const URL = `${RENDER_URL}?${Local_STR}=${encodeURIComponent(Dado_a_Retornar)}`;
        const resposta = await fetch(URL);
        return resposta;
    } catch (erro) {
        throw erro;
    }
}

// Função auxiliar que altera a data recebida para o modelo e UTC de São Paulo.
function Formatar_Data_Sao_Paulo(Data_Entrada) {
    if (!Data_Entrada) return "";
    
    const Data = new Date(Data_Entrada);
    
    if (isNaN(Data.getTime())) return "";

// Retorna a data em formato de string no modelo de data e hora e no UTC de São Paulo.
    return Data.toLocaleString("pt-BR", {
        timeZone: "America/Sao_Paulo"
    });
}

// Função para o lançamento dos alertas
async function enviarNotificacao() {
    if (!("Notification" in window)) {
        alert("Seu navegador não suporta notificações.");
        return;
    }

    const permissao = await Notification.requestPermission();

    if (permissao === "granted") {
        let notificacao = new Notification("Estação Meteorológica", {
            body: dados.alerta[0].mensagem
        });

        notificacao.onclick = () => {
            window.focus();
        };

    } else {
        alert("Permissão para notificações não concedida.");
    }
}

// Função auxiliar que busca os dados na rota "/dados".
async function Buscar_Dados() {
    try {
        const resposta = await fetch(RENDER_URL);
        if (!resposta.ok) {
            throw new Error(`Erro HTTP: ${resposta.status}`);
        }
        // A variável de escopo global recebe a resposta da requisição no formato json. Portanto, todas as outras funções que recebam "dados", serão atualizadas.
        dados = await resposta.json();
        console.log("Dados recebidos:", dados)
    } catch (erro) {
        console.error("Erro ao buscar dados do Flask:", erro);
        return null;
    }
}

// Função auxiliar que usa da biblioteca "chart" para renderizar os gráficos com base nos dados atuais.
function Renderizar_Grafico(historico) {
    // Controle para verificar se o "historico" recebido é uma lista e define um valor. Se for nulo, retorna uma lista vazia. Senão, retorna com os valores de histórico.
    const lista = Array.isArray(historico) ? historico : (historico?.Historico_de_Dados || []);

    // Verifica se a lista possui algum valor dentro dela, senão, retorna um aviso.
    if (!Array.isArray(lista) || lista.length === 0) {
        console.warn("Nenhum histórico disponível para os gráficos.");
        return;
    }

    // Se a biblioteca não existir, para a função.
    if (typeof Chart === "undefined") {
        console.error("A biblioteca Chart.js não foi encontrada.");
        return;
    }

    // Armazena os tipos possíveis de dado, aplicando um nome, uma chave e unidade únicos.
    const Tipos_Possiveis = [
        {
            chave: "temperatura",
            nome: "Temperatura",
            unidade: "°C",
            cor: "#ff0404"
        },
        {
            chave: "umidade",
            nome: "Umidade",
            unidade: "%",
            cor: "#0431fc"
        },
        {
            chave: "pressão",
            nome: "Pressão atmosférica",
            unidade: "hPa",
            cor: "#ff8503"
        },
        {
            chave: "luminosidade",
            nome: "Luminosidade",
            unidade: "",
            cor: "#ffea00"
        },
        {
            chave: "gás",
            nome: "Qualidade do ar (gás)",
            unidade: "",
            cor: "#5e6f69"
        }
    ];

    // Cria o eixo horizontal abaixo dos gráficos com base na data e hora de cada registro.
    const labels = lista.map((item, index) => {
        const data = item.data_hora ?? item.Data_Hora;

        return data? Formatar_Data_Sao_Paulo(data): `Registro ${index + 1}`; 
    });

    // Para cada tipo, desenha um novo gráfico para cada tipo e aplica os valores.
    Tipos_Possiveis.forEach(tipo => {
        const canvas = document.getElementById(
            `graficoHistorico_${tipo.chave}`
        );

        if (!canvas) {
            console.warn(`Canvas não encontrado: graficoHistorico_${tipo.chave}`);
            return;
        }

        // Percorre a lista de dados e extrai os valores correspondentes ao tipo selecionado.
        const valores = lista.map(item => {
            const valor = item[tipo.chave]
                ?? item[tipo.chave === "pressão" ? "pressao" :
                        tipo.chave === "gás" ? "qualidade_ar" :
                        tipo.chave === "temperatura" ? "Temperatura" :
                        tipo.chave === "umidade" ? "Umidade" :
                        "Luminosidade"];

            return valor == null || valor === ""
                ? null
                : Number(valor);
        });

          // Se o gráfico ter sido feito e não for nulo, aplica os valores e o texto inferior com os valores das datas.
        if (Graficos[tipo.chave]) {
            Graficos[tipo.chave].data.labels = labels;
            Graficos[tipo.chave].data.datasets[0].data = valores;
            Graficos[tipo.chave].update();
            return;
        }

        // Nessa parte, personalizamos parte do gráfico com base na lista anteriormente citada de "Tipos_Possiveis", aplicando cor, nome e unidade. 
        Graficos[tipo.chave] = new Chart(canvas.getContext("2d"), {
            type: "line",
            data: {
                labels: labels,
                datasets: [{
                    label: `${tipo.nome} ${tipo.unidade}`,
                    data: valores,
                    borderColor: tipo.cor,
                    backgroundColor: tipo.cor + "30",
                    borderWidth: 2,
                    fill: true,
                    tension: 0.3,
                    spanGaps: false,
                    pointRadius: 3
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                animation: false,
                plugins: {
                    legend: {
                        display: true,
                        labels: {
                            font: {
                                size: 9
                            },
                            boxWidth: 12,
                            padding: 8
                        }
                    }
                },
                scales: {
                    y: {
                        beginAtZero: false,
                        ticks: {
                            font: {
                                size: 10
                            }
                        }
                    },
                    x: {
                        grid: {
                            display: false
                        },
                        ticks: {
                            font: {
                                size: 8
                            },
                            autoSkip: true,
                            // Nessa parte, limitamos a quantidade de "horas" na parte horizontal abaixo do gráfico, podem aparecer. Ou seja, aparecerão um total de 15 horas diferentes, para melhor visualização. 
                            maxTicksLimit: 15,
                            maxRotation: 45,
                            minRotation: 0
                        }
                    }
                }
            }
        });
    });
}


// Função que administra a criação de arquivos CSV com base no dado atual na aplicação.
function Criar_Relatorio(Fonte_de_Dados){ 
    // Busca o botão de exportação do relatório.
    const exportBtn = document.getElementById("btnRelatorio") || Array.from(document.querySelectorAll('button')).find(btn => btn.textContent.includes('Gerar Relatório CSV'));

    if (!exportBtn) {
        console.warn("Botão de gerar relatório não encontrado.");
        return;
    }

    // Evento de quando o botão é clicado. Se não existir uma fonte de dados, para a função.
    exportBtn.onclick = async (e) => {
        e.preventDefault();
        if (!Fonte_de_Dados) {
            alert("Não foi possível carregar os dados para gerar o relatório.");
            return;
        }
        
    //  Verificação da estrutura dos dados recebidos para que "linhasHistórico" sempre receba uma lista.
        let linhasHistorico = [];
        if (Array.isArray(Fonte_de_Dados.Historico_de_Dados) && Fonte_de_Dados.Historico_de_Dados.length > 0) {
            linhasHistorico = Fonte_de_Dados.Historico_de_Dados;
        } else if (Array.isArray(Fonte_de_Dados)) {
            linhasHistorico = Fonte_de_Dados;
        } else {
            linhasHistorico = [Fonte_de_Dados];
        }
    
    // Variável que contém os títulos das colunas
        const reportData = [["Data_Hora", "Estacao", "Temperatura", "Umidade", "Pressao", "Luminosidade", "Gas", "Codigo_HTTP"]];
        
    // Para cada linha de histórico existente, aplica os dados à "reportData".
        linhasHistorico.forEach(item => {
            reportData.push([
                item.data_hora || item.Data_Hora || Fonte_de_Dados.Data_Hora || "",
                Fonte_de_Dados.Nome_Estacao || item.Nome_Estacao || "",
                item.temperatura ?? Fonte_de_Dados.temperatura ?? "",
                item.umidade ?? Fonte_de_Dados.umidade ?? "",
                item.pressão ?? Fonte_de_Dados.pressão ?? "",
                item.luminosidade ?? Fonte_de_Dados.luminosidade ?? "",
                item.gás ?? Fonte_de_Dados.gás ?? "",
                Fonte_de_Dados.Codigo_HTTP || item.Codigo_HTTP || "200"
            ]);
        });

        // Converte cada linha do relatório em texto, separando as colunas por ponto e vírgula.
        let csvRows = reportData.map(linha => linha.join(";"));

        // Junta todas as linhas em uma única string, separando-as por quebras de linha.
        // O \uFEFF adiciona uma marca de identificação para facilitar a leitura de caracteres especiais.
        let csvString = "\uFEFF" + csvRows.join("\n");

        // Cria um arquivo CSV temporário a partir dos dados.
        let blob = new Blob([csvString], { type: 'text/csv;charset=utf-8;' });

        // Gera uma URL temporária para permitir o download do arquivo.
        let url = URL.createObjectURL(blob);

        // Cria um elemento de link HTML para iniciar o download.
        let link = document.createElement("a");

        // Define o endereço do arquivo e o nome que será utilizado no download.
        link.setAttribute("href", url);
        link.setAttribute("download", `relatorio_climatico.csv`);

        // Adiciona o link à página, inicia o download e depois remove o elemento.
        document.body.appendChild(link);
        link.click();
        document.body.removeChild(link);
    };
}

// Atualiza a aba de recebimento com novos dados, caso existam novos dados.
function Atualizar_Recebimento(dados) {
    if(!dados){
        return
    }
    if (dados.Historico_de_Dados && dados.Historico_de_Dados.length > 0) {
        Pegar_Elemento_Por_ID("Recent_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Recent_Station_Data", "Enviou novos dados.", "");
        Pegar_Elemento_Por_ID("Recent_Station_Time",Formatar_Data_Sao_Paulo(dados.Data_Hora ?? dados.data_hora),"");
    } else {
        Pegar_Elemento_Por_ID("Recent_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Recent_Station_Data", "Sem dados.", "");
        Pegar_Elemento_Por_ID("Recent_Station_Time", "Sem atualização.", "");
    }
}

// Atualiza a análise com novos dados, caso existam novos dados.
function Atualizar_Analise(dados) {
    if(!dados){
        return
    }

    if (dados.Historico_de_Dados && dados.Historico_de_Dados.length > 0) {
        Pegar_Elemento_Por_ID("Analytics_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Analytics_Station_Data", "Enviou novos dados.", "");
        Pegar_Elemento_Por_ID("Analytics_Updates_Value", dados.Qtd_Atualizados ?? dados.Historico_de_Dados.length, "");
    } else {
        Pegar_Elemento_Por_ID("Analytics_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Analytics_Station_Data", "Sem dados.");
        Pegar_Elemento_Por_ID("Analytics_Updates_Value", dados.Qtd_Atualizados ?? 0, "");
        Pegar_Elemento_Por_ID("Analytics_Time", "Sem atualização.", "");
    }
}
// Atualiza a tabela de históricos com os dados recebidos.
function Atualizar_Tabela_de_Historicos(dados) {

    // Verifica se existem dados recebidos. Caso contrário, encerra a função.
    if (!dados) {
        return;
    }

    // Obtém o histórico de dados. Caso não exista, utiliza um array vazio.
    Registro_do_Historico = dados.Historico_de_Dados ?? [];

    // Armazena os registros do histórico em uma variável para facilitar o acesso.
    let Tabela_Historico_de_Dados = Registro_do_Historico;

    // Obtém a quantidade de registros, considerando o índice do último elemento.
    let Tamanho_Total = Tabela_Historico_de_Dados.length - 1;

    // Procura o corpo da primeira tabela na página.
    let tbody = document.querySelector(".recent-orders tbody");

    // Caso não encontre, procura o corpo de uma segunda tabela.
    if (!tbody) {
        tbody = document.querySelector(".table-card tbody");
    }

    // Verifica se alguma tabela foi encontrada. Caso contrário, exibe um erro e encerra a função.
    if (!tbody) {
        console.error("Tabela não encontrada.");
        return;
    }

    // Limpa o conteúdo atual da tabela antes de inserir os novos registros.
    tbody.innerHTML = "";

    // Verifica se o histórico está vazio.
    if (Tabela_Historico_de_Dados.length === 0) {

        // Cria uma linha informando que não existem registros disponíveis.
        let tr = document.createElement("tr");
        tr.innerHTML = `<td colspan="4">Nenhum registro encontrado.</td>`;

        // Adiciona a mensagem à tabela.
        tbody.appendChild(tr);

    } else {

        // Chama a função responsável por percorrer os registros e preencher a tabela.
        // Utiliza 10 registros para a primeira tabela ou 20 para a segunda.
        Looping_Registros(
            Tamanho_Total,
            tbody.closest(".recent-orders") ? 10 : 20,
            0,
            tbody,
            Tabela_Historico_de_Dados
        );
    }
}
// Looping que serve para aplicar os últimos registros inseridos.
function Looping_Registros(Tamanho_Total, Limite_Repeticoes, Contador_Registros, tbody, Tabela_Historico_de_Dados) {
    // É um while "decrescente". Ou seja, ele vai do último elemento até o "n"gésimo registro passado em "Limite_Repeticoes".
    while (Limite_Repeticoes > Contador_Registros && Tamanho_Total >= 0) {
        const Registro = Tabela_Historico_de_Dados[Tamanho_Total];

        const Data_Registro = Registro.data_hora ?? Registro.Data_Hora ?? Registro.created_at;
        const Data = Data_Registro ? new Date(Data_Registro) : null;
        const data_formatada = Data && !isNaN(Data.getTime())
            ? Data.toLocaleString("pt-BR")
            : "";

        let tr = document.createElement("tr");

        /* Cria uma nova "linha" com nome da estação, o Id do registro atual e a data formatada.
           A base para pegar essa informação é o "Registro".
        */
        tr.innerHTML = `
            <td>${dados.Nome_Estacao ?? ""}</td>
            <td>${Registro.Id_Estacao ?? ""}</td>
            <td>${data_formatada}</td>
            <td class="success">${dados.Codigo_HTTP ?? "200 OK"}</td>
        `;

        tbody.appendChild(tr);
        Tamanho_Total--;
        Contador_Registros++;
    }
}

// Função auxiliar para pegar o elemento pelo ID e aplicar o valor passado,  à esse elemento.
function Pegar_Elemento_Por_ID(ID, Valor_Preencher, Sinal) {
    const Elemento_HTML = document.getElementById(ID);

    if (!Elemento_HTML) {
        console.error("Elemento não encontrado:", ID);
        return;
    }

    Elemento_HTML.textContent =
        `${Valor_Preencher ?? ""} ${Sinal ?? ""}`.trim();
}

// Função auxiliar para limpar a tabela de históricos.
function Limpar_Tabela() {
    let tbody = document.querySelector(".recent-orders tbody");

    if (!tbody) {
        tbody = document.querySelector(".table-card tbody");
    }

    if (tbody) {
        tbody.innerHTML = "";
    }
}

/* Função auxiliar. Atualiza o progresso do círculo ao redor das variáveis.
   Determina o valor máximo com base na variável, permitindo que o preenchimento seja dinâmico e não fixo.
*/
function Atualizar_Progresso_Circulo(seletorClasse, valor, valorMaximo) {
    const circulo = document.querySelector(`.${seletorClasse} svg circle`);
    if (!circulo) return;

    const numero = Number(valor);
    const maximo = Number(valorMaximo);

    if (
        valor === null ||
        valor === undefined ||
        valor === "" ||
        !Number.isFinite(numero) ||
        !Number.isFinite(maximo) ||
        maximo <= 0
    ) {
        circulo.style.strokeDashoffset = "226";
        return;
    }

    const porcentagem = Math.min(Math.max((numero / maximo) * 100, 0), 100);
    const raio = Number(circulo.getAttribute("r"));
    const circunferencia = 2 * Math.PI * raio;

    circulo.style.strokeDasharray = circunferencia;
    circulo.style.strokeDashoffset = circunferencia - (circunferencia * porcentagem) / 100;
}

// Função auxiliar. Converte a temperatura de Celsius para Fahrenheit. Troca o sinal e faz a conversão correta.
function Converter_Temperatura(valorCelsius) {
    if (
        valorCelsius === null ||
        valorCelsius === undefined ||
        valorCelsius === "" ||
        !Number.isFinite(Number(valorCelsius))
    ) {
        return { valor: "", sinal: "°C" };
    }

    const unidadeGuardada = localStorage.getItem("pref_temp_unit");

    if (unidadeGuardada === "Fahrenheit (°F)") {
        const fahrenheit = (Number(valorCelsius) * 9 / 5) + 32;

        return {
            valor: fahrenheit.toFixed(1),
            sinal: "°F"
        };
    }

    return {
        valor: valorCelsius,
        sinal: "°C"
    };
}

// Função auxiliar que identifica os elementos do HTML e aplica os dados neles.
function Agrupar_Elementos(dados) {
    if (!Pausar_Atualização) {
        Atualizar_Recebimento(dados);
        Atualizar_Analise(dados);
    }

    //
    const tempConvertida = Converter_Temperatura(dados.temperatura);

    // Variáveis auxiliares para ajustar a porcentagem dos valores recebidos.
    let pctTemp = dados.temperatura != null ? Math.min(Number(dados.temperatura) || 0, 100) : 0;
    let pctUmid = Number(dados.umidade) || 0;
    let pctPressao = dados.pressão != null ? (Number(dados.pressão) / 1100) * 100 : 0;
    let pctLuz = Number(dados.luminosidade) || 0;
    let pctGas = Number(dados.gás) || 0;

    // Função que pega o elemento pelo id (string) e aplica os valores e o sinal de preferência (último parâmetro).
    Pegar_Elemento_Por_ID("temperatura", tempConvertida.valor, tempConvertida.sinal);
    Pegar_Elemento_Por_ID("%_temperatura", Math.round(pctTemp), "%");

    Pegar_Elemento_Por_ID("umidade", dados.umidade, "%");
    Pegar_Elemento_Por_ID("%_umidade", Math.round(pctUmid), "%");

    Pegar_Elemento_Por_ID("pressão", dados.pressão, "hPa");
    Pegar_Elemento_Por_ID("%_pressão", Math.round(pctPressao), "%");

    Pegar_Elemento_Por_ID("luminosidade", dados.luminosidade, "");
    Pegar_Elemento_Por_ID("%_luminosidade", Math.round(pctLuz), "%");

    Pegar_Elemento_Por_ID("gás", dados.gás, "");
    Pegar_Elemento_Por_ID("%_gas", Math.round(pctGas), "%");

    // Função que atualiza o preenchimento dos "círculos" que rodeam o valor da variável.
    Atualizar_Progresso_Circulo("temperature", pctTemp, 50);
    Atualizar_Progresso_Circulo("humidity", pctUmid, 100);
    Atualizar_Progresso_Circulo("windspeed", pctPressao, 100);
    Atualizar_Progresso_Circulo("luz", pctLuz, 5000);
    Atualizar_Progresso_Circulo("Gás", pctGas, 100);
}

// Função auxiliar para retornar os dados ao Back-End. Recebe a informação e uma String para criar o caminho (url).
async function Retornar_Dados_ao_Back(Dado_a_Retornar, Local_STR) {
    try {
        const URL = `${RENDER_URL}?${Local_STR}=${encodeURIComponent(Dado_a_Retornar)}`;
        const resposta = await fetch(URL);
        return resposta;
    } catch (erro) {
        throw erro;
    }
}

// Função para filtro das informações com base na data selecionada pelo usuário.
async function Filtrar_por_Data() {
    Input_Data = Filtro_de_Data
    if (!Input_Data) {
        console.error("Campo de data não encontrado.");
        return;
    }

    let Data_Selecionada = Input_Data.value;

    if (!Data_Selecionada) {
        // Se a data não existir ou for selecionada, atualiza com os dados padrões mais recentes.
        Pausar_Atualização = false;
        Atualizar_Estado(dados)
        return;
    }

    Pausar_Atualização = true;

    // Envia a data para o Back-End, esperando um retorno do mesmo. Os dados exibidos no Dash são os últimos registrados no dia escolhido.
    try {
        // Envia a data ao Back-End.
        const Resposta_Filtro = await Retornar_Dados_ao_Back(Data_Selecionada,"data");
        // Espera o retorno da resposta do filtro.
        const dados_filtrados = await Resposta_Filtro.json();
        console.log("todos os dados:", dados_filtrados)
        // Separa os últimos dados do arquivo json recebido.
        const Ultimo_Registro = dados_filtrados.at(-1);

        if (!Array.isArray(dados_filtrados)) {
            console.error("Resposta inesperada do Flask:", dados_filtrados);
            return;
        }
        // Se tiver o último registro, atualiza com base nos últimos dados recebidos do filtro. 
        if(Ultimo_Registro){
        Atualizar_Estado(Ultimo_Registro)
        }
        // Se não, atualiza com os dados base.
        else{
            Filtro_de_Data.value = "";
            Atualizar_Estado(dados)
        }
        
    } catch (erro) {
        console.error("ERRO NO FILTRO:", erro);
    // E, nessa parte, temos um formato de "duração" da tela de filtro. Depois do tempo específicado, a aplicação volta para o funcionamento padrão.
    } finally {
        setTimeout(() => {
            Pausar_Atualização = false;
            Atualizar_Estado(dados);
        }, 30000);
    }
}

// Função que inicia o funcionamento da aplicação e a alimentação com os dados mais recentes.
async function Iniciar_Programa() { 
    /* Busca os dados, chamando a função "Buscar_Dados" que atualiza uma variável global "dados".
    */
    await Buscar_Dados();
    await Atualizar_Estado(dados)
    Criar_Relatorio(dados);

    if(dados.estado_alerta){
        enviarNotificacao()
    }

    // No caso de não haver um filtro, espera por um total de 10 segundos antes de fazer uma nova requisição ao Back-End.
    setInterval(() => {
        if (!Pausar_Atualização) {
            Buscar_Dados();
            Atualizar_Estado(dados)
        }
    }, 5000);
}

/* Função com o próposito de atualizar todos os conteúdos da aplicação com base em uma "Fonte_de_Dados".
   Quando em processo de atualização comum, a fonte de dados é a variável global "dados". Agora, no caso de haver um filtro, essa função é chamada com um argumento diferente.
*/
async function Atualizar_Estado(Fonte_de_Dados){
    // Atualiza todos os elementos com base no argumento passado.
    Agrupar_Elementos(Fonte_de_Dados);
    Atualizar_Analise(Fonte_de_Dados);
    Atualizar_Recebimento(Fonte_de_Dados);
    Atualizar_Tabela_de_Historicos(Fonte_de_Dados);
    Renderizar_Grafico(Fonte_de_Dados);
    Criar_Relatorio(Fonte_de_Dados);
}

// Inicia o programa ao iniciar o looping de atualização.
Iniciar_Programa();
```

</details>
<details>
<summary> Mapa.js </summary>

```csharp
// Define o endereço da API que fornece os dados da estação meteorológica.
const RENDER_URL = "https://projetos-estacao-meteorol-gica.onrender.com/dados";

// Declara uma variável para armazenar os dados recebidos da API.
let dados;

// Busca os dados da API e armazena a resposta recebida.
async function Buscar_Dados() {

    // Realiza uma requisição à API utilizando o método fetch().
    const resposta = await fetch(RENDER_URL);

    // Verifica se a resposta foi recebida corretamente.
    // Caso contrário, lança um erro com o código HTTP.
    if (!resposta.ok) {
        throw new Error(`Erro HTTP: ${resposta.status}`);
    }

    // Converte a resposta da API para o formato JSON.
    dados = await resposta.json();

    // Exibe os dados recebidos no console para conferência.
    console.log(dados);

    // Retorna os dados obtidos.
    return dados;
}

// Busca o elemento do HTML onde o mapa será exibido.
const mapElement = document.getElementById('map');

// Verifica se o elemento do mapa existe e se a biblioteca Leaflet está disponível.
if (mapElement && typeof L !== 'undefined') {

    // Inicializa o mapa com as coordenadas iniciais e o nível de aproximação.
    const map = L.map('map').setView([-23.4735, -46.7231], 13);

    // Define o estilo visual do mapa utilizando imagens fornecidas pelo serviço ArcGIS.
    L.tileLayer(
        'https://server.arcgisonline.com/ArcGIS/rest/services/World_Street_Map/MapServer/tile/{z}/{y}/{x}',
        {
            attribution: 'Tiles &copy; Esri'
        }
    ).addTo(map);

    // Busca os dados da estação meteorológica antes de adicionar sua localização ao mapa.
    Buscar_Dados()

        // Executa quando os dados da API são recebidos corretamente.
        .then(dados => {

            // Organiza as informações da estação em um objeto.
            const station = {
                name: dados.Nome_Estacao ?? "Estação sem nome",
                status: "Online",
                temp: dados.temperatura ?? "--",
                lat: Number(dados.latitude),
                lng: Number(dados.longitude)
            };

            // Verifica se a latitude e a longitude recebidas são válidas.
            if (isNaN(station.lat) || isNaN(station.lng)) {
                console.error("Coordenadas inválidas:", station);
                return;
            }

            // Cria um marcador no mapa utilizando as coordenadas da estação.
            // Também adiciona uma janela com o nome, status e temperatura da estação.
            L.marker([station.lat, station.lng])
                .addTo(map)
                .bindPopup(`
                    <b>${station.name}</b><br>
                    Status: ${station.status}<br>
                    Temp: ${station.temp} °C
                `);
        })

        // Caso ocorra algum erro durante a busca ou processamento dos dados,
        // exibe uma mensagem no console.
        .catch(erro => {
            console.error("Erro ao carregar dados da estação:", erro);
        });

    // Aguarda 300 milissegundos e recalcula o tamanho do mapa.
    // Isso ajuda a corrigir problemas de exibição quando o mapa é carregado.
    setTimeout(() => {
        map.invalidateSize();
    }, 300);
}
```

</details>
<details>
<summary> Preferencias.js </summary>

```csharp
// Busca os elementos de configuração no HTML da página:
// seletor de unidade de temperatura, caixa de seleção de notificações
// e botão responsável por salvar as alterações.
const tempUnitSelect = document.querySelector('.settings-form select');
const emailCheckbox = document.querySelector('.settings-form input[type="checkbox"]');
const saveSettingsBtn = Array.from(document.querySelectorAll('button')).find(btn => btn.textContent.includes('Salvar Alterações'));

// Verifica se os campos de preferência existem antes de recuperar os valores salvos.
if (tempUnitSelect && emailCheckbox) {

    // Recupera as preferências armazenadas anteriormente no localStorage.
    const savedUnit = localStorage.getItem('pref_temp_unit');
    const savedEmailNotif = localStorage.getItem('pref_email_notif');

    // Preenche os campos com as preferências salvas, caso existam.
    if (savedUnit) tempUnitSelect.value = savedUnit;

    // Converte o valor armazenado em JSON para booleano e atualiza a caixa de seleção.
    if (savedEmailNotif !== null) emailCheckbox.checked = JSON.parse(savedEmailNotif);
}

// Verifica se o botão de salvar foi encontrado.
if (saveSettingsBtn) {

    // Adiciona um evento de clique ao botão para salvar as preferências.
    saveSettingsBtn.addEventListener('click', (e) => {

        // Impede o comportamento padrão do botão, como o envio de um formulário.
        e.preventDefault();

        // Verifica se os campos de preferência existem.
        if (tempUnitSelect && emailCheckbox) {

            // Armazena a unidade de temperatura escolhida pelo usuário no localStorage.
            localStorage.setItem('pref_temp_unit', tempUnitSelect.value);

            // Armazena a preferência de notificações por e-mail.
            localStorage.setItem('pref_email_notif', emailCheckbox.checked);

            // Exibe uma mensagem confirmando que as preferências foram salvas.
            alert('Preferências salvas com sucesso!');
        }
    });
}
```

</details>
</details>


</details>
