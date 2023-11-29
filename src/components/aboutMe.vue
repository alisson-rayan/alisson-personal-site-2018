<template>
    <div class="about">
        <div class="person">
            <div class="image" />
            <div class="info">
                <h1 class="name">Alisson<span class="-bold">Rayan</span></h1>
                <h2 class="office">Front<span class="-bold">End</span> Dev</h2>
                <div class="actions">
                    <button class="btn" @click="downloadCurriculum">Baixar currículo</button>
                    <button class="btn" @click="$emit('open-curriculum')">Vizualizar currículo</button>
                </div>
            </div>
        </div>
        <div class="contact">
            <hr class="divider">
            <p class="email"><span class="-bold">alisson.rayan</span>@outlook.com</p>
            <p class="tel"><span class="-bold">(11)</span>97672-1914</p>
            <div class="social-media">
                <a class="media" href="https://github.com/alissonrayan" target="_blank">Git<span class="-bold">hub</span></a>
                <a class="media" href="https://codepen.io/alissonrayan" target="_blank">Code<span class="-bold">Pen</span></a>
                <a class="media" href="https://www.linkedin.com/in/alisson-rayan-nogueira-gabriel-112838131" target="_blank">Linked<span class="-bold">in</span></a>
                <a class="media" href="https://www.instagram.com/_silentstar/" target="_blank">Insta<span class="-bold">gram</span></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        downloadCurriculum () {
            var link = document.createElement("a");
            link.href = 'https://drive.google.com/uc?authuser=0&id=13FEKhMSkpUi_k2t0NSGSZYzZ2Gw9e2Ol&export=download';
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
        }
    }
}
</script>

<style lang="scss">
    .about {
        & >.person {
            display: flex;
            z-index: 20;
            @media only screen and (max-width: 768px) {
                flex-direction: column;
                align-items: center;
                padding-top: 20px;
            }
            & >.image {
                width: 200px;
                height: 200px;
                border-radius: 50%;
                background-image: url('../assets/pic.png');
                background-position: center;
                background-size: cover;
                
                @media only screen and (min-width: 768px) {
                margin-right: 15px;
                }
            }
            & >.info {
                & >.name {
                    text-align: start;
                    color: #C2C0C9;
                    font-weight: 100;
                    @media only screen and (max-width: 768px) {
                        text-align: center;
                    }
                }
                & >.office {
                    text-align: start;
                    font-size: 18px;
                    color: #C2C0C9;
                    font-weight: 100;
                    @media only screen and (max-width: 768px) {
                        text-align: center;
                    }
                }
                & >.actions {
                    & >.btn {
                        background: transparent;
                        color: #C2C0C9;
                        border-radius: 20px;
                        padding: 6px;
                        min-width: 130px;
                        cursor: pointer;

                        &:not(:last-child) {
                            margin-right: 5px;
                        }
                    }
                }
            }
        }
        & >.contact {
            padding: 0 20px;

            & >.email, .tel {
                text-transform: uppercase;
                color: #C2C0C9;
            }
            & >.divider {
                border: 1px solid #C2C0C9;
                opacity: .1;
            }
            & >.social-media {
                display: flex;
                justify-content: space-around;
                margin-top: 30px;
                
                & >.media {
                    font-size: 16px;
                    position: relative;
                    margin-top: 3px;
                    text-transform: uppercase;
                    color: #C2C0C9;
                    font-weight: 100;
                    text-decoration: none;
                    &:not(:last-child) {
                        margin-right: 10px;
                    }
                    &:after {
                        bottom: 0;
                        content: "";
                        display: block;
                        height: 1px;
                        left: 50%;
                        position: absolute;
                        background: #C2C0C9;
                        transition: width 0.3s ease 0s, left 0.3s ease 0s;
                        width: 0;
                    }
                    &:hover:after { 
                        width: 100%; 
                        left: 0; 
                    }
                }
            }
        }
        .-bold {
        color: #C2C0C9;
        font-weight: 600;
        }
    }
</style>