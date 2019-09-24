<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=<device-width>, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>

<body>
    <div id="root">

    </div>
    <button onclick="lavSide()">klik mig</button>
    <button onclick="beregn()">beregn co2</button>
</body>
<script>
    function beregn() {
        //skaf referance til root element
        let side = document.getElementById("root");
    }


    function lavSide() {
        //skaf referance til root element
        let side = document.getElementById("root");
        //opret textbox
        let textboks = document.createElement("input");
        textboks.type = Number;
        textboks.id="sTog"
        textboks.placeholder ="shriv hvor mange km  stog"

        //opret et overskrifts elememnt
        let overskrift = document.createElement("h1");
        //giv overskrift en inner html
        overskrift.innerHTML = "Co2 beregner";
        //insæt overskriften under root
        side.appendChild(overskrift);
        //sæt input feltet på siden
        side.appendChild(textboks)
    }
</script>

</html>
