# CSS Static Pie Chart
Pie chart practice #1

<code>
.pie-chart{

    position: absolute; top: 0px; left: 0px;
    width: 120px; height: 120px; border: 0px solid transparent;
    border-radius: 50%;
    background-color: transparent;
    text-align: center;
    line-height: 120px;
    color: orange;
    cursor: pointer;
}

.pie-chart::before,
.pie-chart::after{

    content:'';
    position: absolute; top: 0px; left: 0px;
    width: 100px; height: 100px; border: 10px solid orange;
    border-radius: 50%;
}

.pie-chart::before{

    clip: rect(0px, 60px, 120px, 0px);
}
.pie-chart::after{

    clip: rect(0px, 120px, 120px, 60px);
    transform: rotate(287deg);
}
</code>
