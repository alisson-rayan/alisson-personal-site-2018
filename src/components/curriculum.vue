<template>
    <div class="curriculum">
        <button 
            class="back"
            @click="$emit('close')"
        >
            Voltar
        </button>
        <h2>ALISSON RAYAN NOGUEIRA GABRIEL</h2>
        <p>
            Brasileiro, solteiro, 21 anos<br />
            Avenida Artemio Dorsa, 181<br />
            Jd. São José – Bragança Paulista – São Paulo<br />
            Telefone: (11)97672-1914 / E-mail: alisson.rayan@outlook.com
        </p>

        <h2>OBJETIVO</h2>
        <p>Programador: front-end</p>

        <h2>FORMAÇÃO</h2>

        <ul>
            <li>
                Análise e desenvolvimento de sistemas - Instituto Federal de São Paulo, Campus Bragança Paulista(2016 - atualmente)
            </li>
            <li>
                Técnico em Informática - Senac Minas Gerais - Pouso Alegre(2014 - 2016)
            </li>
        </ul>

        <h2>EXPERIÊNCIA PROFISSIONAL</h2>
        <ul>
            <li>
                27/09/2019 até o momento – Juros Baixos Cargo: Desenvolvedor Front-end Pleno<br />
                Principais atividades: Criação de sites, manutenção do sistema.
            </li>
            <li>
                02/04/2018 á 24/06/2019 – Convenia atividades de internet<br />
                Cargo:Desenvolvedor Web Jr. Principais atividades: Criação de Websites, manutenção de sistemas web, front-end utilizando diversas libs.
            </li>
            <li>
                01/08/2016 á 07/08/2017 – Quicktech Cargo: Desenvolvedor Web<br />
                Principais atividades: Criação de Websites, manutenção de sistemas web, front-end e back-end utilizando diversas linguagens e tecnologias.
            </li>
        </ul>

        <h2>INFORMAÇÕES ADICIONAIS</h2>
        <p>CNH - AB - Veículo Próprio - Disponibilidade para trabalho Remoto - Disponibilidade de mudança e viagem.</p>

        <h2>QUALIFICAÇÕES E ATIVIDADES PROFISSIONAIS</h2>
        <ul>
            <li>
                Atividade de Extensão para o Instituto Federal Campus Bragança Paulista, Website para o grupo de pesquisa do Campus(março/2016 - dezembro/2016).
            </li>
            <li>
                Curso Web Design (Upnet, 2011).
            </li>
            <li>
                Curso Informática básica (Gigabyte Cursos, 2009-2010).
            </li>
            <li>
                Cursos Relacionados a programação online(Udemy, CodeWars, Udacity).
            </li>
        </ul>
        
        <h2>PRINCIPAIS ATIVIDADES:</h2>
        <ul>
            <li>Implementar novos sites</li>
            <li>Implementar novas features</li>
            <li>Dar manutenção corrigir bugs e implementar novas melhorias.</li>
        </ul>

        <h2>HABILIDADES:</h2>
        <p>
            - HTML(avançado) - CSS(avançado) - JavaScript(Intermediário) - Vue JS(avançado) - Nuxt - Typescript Angular - React - ES6 - UX Design - Bootstrap/Foundation - Desenvolvimento Responsivo nativo  - PHP - Wordpress - Java(básico) - C# - SASS - RCSS - BEM CSS - JADE - Desenvolvimento em OSX/Linux/Windows - jQuery - GIT - Gulp/Grunt - SCRUM - MySql - MongoDB - Firebase - Photoshop
        </p>

        <h2>OBSERVAÇÕES:</h2>
            <p>Preferência para realizar teste prático para demonstrar minhas habilidades.</p>

        <h2>PRETENSÃO SALARIAL:</h2>
        <ul>
            <li>À partir de 8.500,00</li>
        </ul>
        <br />
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
    @mixin custom-scroll-bar {
        &::-webkit-scrollbar-track {
            -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
            border-radius: 10px;
            background-color: transparent;
        }

        &::-webkit-scrollbar {
            width: 5px;
            background-color: transparent;
        }

        &::-webkit-scrollbar-thumb {
            border-radius: 10px;
            -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3);
            background-color: rgba(#C2C0C9, .5);
        }
    }
    .curriculum {
        overflow-y:scroll; 
        position:relative;
        height: 400px;
        max-width: 600px;
        text-align: left;

        @media only screen and (max-width: 768px) {
            height: 100%;
            padding: 15px;
        }
        @include custom-scroll-bar;
        
        & >.back {
            background: transparent;
            color: #C2C0C9;
            border-radius: 20px;
            padding: 6px;
            min-width: 130px;
            cursor: pointer;
        }
        & > h2 {
            font-size: 20px;
            font-family: 'Courier New', Courier, monospace;
            color: #C2C0C9;
            font-weight: 600;
        }
        & > p {
            padding-left: 20px;
            font-size: 14px;
            color: rgba(#C2C0C9, .8);
            font-weight: 200;
        }
        & > ul {
            padding-left: 20px;
            & > li {
                font-size: 14px;
                color: rgba(#C2C0C9, .8);
                font-weight: 200;
            }
        }
        
    }
</style>