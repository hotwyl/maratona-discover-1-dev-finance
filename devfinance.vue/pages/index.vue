<template>
  <div class="body">
    <header>
        <h1 id="logo">dev.finance$</h1>
    </header>

    <main class="container">
        <section id="balance">
            <h2>Balanço</h2>

            <div class="card">
                <h3>Entradas</h3>
                <p>R$ 5.000,00</p>
            </div>

            <div class="card">
                <h3>Saídas</h3>
                <p>R$ 2.000,00</p>
            </div>

            <div class="card total">
                <h3>Total</h3>
                <p>R$ 3.000,00</p>
            </div>
        </section>

        <section id="transaction">
            <h2>Transações</h2>

            <table id="data-table">
                <thead>
                <tr>
                    <th>Descrição</th>
                    <th>Valor</th>
                    <th>Data</th>
                </tr>
                </thead>
                <tbody>
                <tr>
                    <td class="description">Luz</td>
                    <td class="expense">-R$ 500,00</td>
                    <td class="date">23/01/2021</td>
                </tr>
                <tr>
                    <td class="description">Criação de Website</td>
                    <td class="income">R$ 5.000,00</td>
                    <td class="date">23/01/2021</td>
                </tr>
                <tr>
                    <td class="description">Internet</td>
                    <td class="expense">-R$ 500,00</td>
                    <td class="date">23/01/2021</td>
                </tr>
                </tbody>
            </table>
        </section>
    </main>

    <footer>
        <p>dev.finance$</p>
    </footer>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

/* Global =============================*/
:root{
    --dark-blue: #363f5f;
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.body{
    background: #f0f2f5;
    font-family: 'Poppins', sans-serif;
}

.container{
    width: min(90vw, 800px);

    margin: auto;
}

/* Title =============================*/
h2{
    margin-top: 3.2rem;
    margin-bottom: 0.8rem;
    color: var(--dark-blue);

    font-weight: normal;
}

/* Header =============================*/
header{
    background: #2D4A22;
    padding: 2rem 0 10rem;
    text-align: center;
}

#logo{
    color: #fff;
    font-weight: 100;
}

/* Balance =============================*/
#balance{
    margin-top: -8rem;
}

#balance h2{
    color: white;
    margin-top: 0;
}

/* Cards =============================*/
.card{
    background: white;
    padding: 1.5rem 2rem;
    border-radius: 0.25rem;

    margin-bottom: 2rem;

    color: var(--dark-blue);
}

.card h3{
    font-weight: normal;
    font-size: 1rem;
}

.card p{
    font-size: 2rem;
    line-height: 3rem;

    margin-top: 1rem;
}

.card.total{
    background: #49AA26;
    color: white;
}

/* Table =============================*/
#data-table{
    width: 100%;
    border-spacing: 0 0.5rem;
    color: #969cb3;
}

table thead tr th:first-child,
table tbody tr td:first-child{
    border-radius: 0.25rem 0 0 0.25rem;
}

table thead th {
    background: white;

    font-weight: normal;
    padding: 1rem 2rem;

    text-align: left;
}

table tbody tr{
    opacity: 0.7;
}

table tbody tr:hover{
    opacity: 1;
}

table tbody td{
    background: white;

    padding: 1rem 2rem;
    font-weight: normal;
}

td.description{
    color: var(--dark-blue)
}

td.income{
    color: #12a454
}

td.expense{
    color: #e92929
}

/* Footer =============================*/
footer{
    text-align: center;
    padding: 4rem 0 2rem;
    color: var(--dark-blue);

    opacity: 0.6;
}
</style>

<script>
export default {
  name: 'IndexPage'
}
</script>
