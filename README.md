# septimo-desafio-ignacio-cordoba

<!-- memberships.scss: uso de @extend -->
.memberships-basic {
    ul {
        list-style-type: none;
        text-align: center;
    }

    a {
        border: solid #eb5e28;
        border-radius: 8px;
        font-size: 20px;
        background: #eb5e28;
        font-weight: bolder;
        color: white;
        text-decoration: none;
        padding: 5px;

        &:hover {
            font-size: larger;
        }
    }

}

.memberships-full {
    @extend .memberships-basic;
}

<!-- our-gyms-scss: uso de mapa -->

$sedes: (
    belgrano,
    boedo,
    caballito,
    palermo,
    recoleta,
    vicentelopez,
);

@each $sede in $sedes {
    .our-gyms-branchs-#{$sede} {
        text-align: center;
        font-weight: 600;
    }
}

<!-- memberships.scss: uso de mixin (no le encontré demasiada utilidad para mi página) -->

@mixin fontstyle {
    color: white;
    font-size: 20px;
    font-weight: bold;
}

.memberships-title {

    h3 {
        @include fontstyle;
        text-align: center;
    }

    p {
        font-size: 20px;
        padding-top: 20px;
        color: white;
        text-align: center;
    }
}

<!-- index.html: agregué keywords y descripción -->

    <meta name="keywords" content="Gimnasio, Planes, Entrenamiento, Musculacion, Ejercicio, Fitness, Deporte">

    <meta name="description" content="Somos el gimnasio con más prestigio del país. ¡No dudes en conocer nuestras sedes, charlar con nuestros asesores y descubrir todo lo que tenemos para ofrecerte!">

<!-- join.html: agregué keywords y descripción -->

    <meta name="keywords" content="Gimnasio, Socio, Pago, Plan, Membresia">

    <meta name="description" content="Elegí tu plan y sucursal, asociate y ¡comenzá el cambio que estás buscando!">

<!-- our-gyms.html: agregué keywords y descripción -->

    <meta name="keywords" content="Gimnasio, Sede, Sucursal, Direccion, Horarios">
 
    <meta name="description" content="Conocé nuestras sedes, instaladas con equipamiento de último modelo para que tu entrenamiento sea óptimo">

<!-- classes.html: agregué keywords y descripción -->

    <meta name="keywords" content="Gimnasio, Clases, Horarios, Dias, Boxeo, GAP, Abdominales, Zumba, Estiramiento">

    <meta name="description" content="Te invitamos a conocer todas las clases que tenemos para ofrecerte">

<!-- faq.html: agregué keywords y descripción -->

    <meta name="keywords" content="Gimnasio, Preguntas, Frecuentes, Consultas, Respuestas">

    <meta name="description" content="¿Tenés alguna duda? No dudes en ingresar y consultar nuestras preguntas frecuentes o contactarnos para que podamos ayudarte.">