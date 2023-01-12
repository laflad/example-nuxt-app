<template>
    <div class="grid">
        <div class="colorcard" :style="'background-color: #'+color.Hex" v-for="(color,id) in colors" :key="id">
            <h3 :class="{darktext:color.hasDarkText}" class="colortitle">{{ color.Name }}</h3>
            <span :class="{darktext:color.hasDarkText}">Hex #{{ color.Hex }}</span>
            <span :class="{darktext:color.hasDarkText}">RGB: {{ color.RGB }}</span>

        </div>
    </div>

</template>

<script>
export default {
    data() {
        return {
            colors: [
                {
                    Name: "Lagoon",
                    Hex: "006887",
                    hasDarkText: false,
                    RGB: "0, 104, 135",
                    Purpose: "Main brand color"
                },
                {
                    Name: "Mist",
                    Hex: "8cd7ed",
                    hasDarkText: true,
                    RGB: "140, 215, 237",
                    Purpose: "Use for dark font when Lagoon is too dark"
                },
                {
                    Name: "Sky",
                    Hex: "288bf3",
                    hasDarkText: false,
                    RGB: "40, 139, 243",
                    Purpose: "Complimentary color"

                },
                {
                    Name: "Abyss",
                    Hex: "1e2829",
                    hasDarkText: false,
                    RGB: "48, 47, 45",
                    Purpose: "Compliments Lagoon well"

                },
                {
                    Name: "Arcadia",
                    Hex: "33302c",
                    hasDarkText: false,
                    RGB: "51, 48, 44",
                    Purpose: "Neutral dark color for fonts"
                },
                {
                    Name: "Roman",
                    Hex: "ed5f5f",
                    hasDarkText: false,
                    RGB: "237, 95, 95",
                    Purpose: "Alert color to use for attention grabbing"
                },
                {
                    Name: "Whisper",
                    Hex: "dce4e6",
                    hasDarkText: true,
                    RGB: "171, 177, 178",
                    Purpose: "Neutral light background color"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.colorcard {
    border-radius: 5px;
    height: 130px;
    display: flex;
    flex-direction: column;
    align-items: left;
    justify-content: end;
    color: white;
    padding: 1rem;
    line-height: 15px;
    font-size: small;
    h3 {
        line-height: 20px;
    }
}

.colortitle {
    text-decoration: solid;
}
.darktext {
    color: black;
}
.grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-column-gap: 30px;
    grid-row-gap: 30px;
}

.colorcard:hover {
    scale: (1.05);
}

.colorcard {
    transition: 0.2s ease;
}
</style>