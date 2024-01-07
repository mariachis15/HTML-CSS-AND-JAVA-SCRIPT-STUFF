document.addEventListener("DOMContentLoaded", function () {
    const colorPalette = [
        "#1f77b4", "#aec7e8", "#ff7f0e", "#ffbb78", "#2ca02c",
        "#98df8a", "#d62728", "#ff9896", "#9467bd", "#c5b0d5",
        "#8c564b", "#c49c94", "#e377c2", "#f7b6d2", "#7f7f7f",
        "#c7c7c7", "#bcbd22", "#dbdb8d", "#17becf", "#9edae5",
        "#393b79", "#5254a3", "#6b6ecf", "#9c9ede", "#637939",
        "#8ca252", "#b5cf6b", "#cedb9c", "#8c6d31", "#bd9e39"
    ];

    const colorContainer = document.getElementById("color-container");

    for (let i = 0; i < colorPalette.length - 1; i+=2) {
        const colorBox = document.createElement("div");
        colorBox.className = "color-box";
        colorBox.style.background = `linear-gradient(to bottom right, ${colorPalette[i]}, ${colorPalette[i+1]})`;
        colorContainer.appendChild(colorBox);
    }
});
