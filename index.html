<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <title>อาหารที่แนะนำเพื่อสุขภาพ</title>
    <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #3e0cf1;
            --secondary-color: #d63384;
            --button-primary: #04aa6a;
            --button-hover: #028a55;
            --button-secondary: #2196f3;
            --button-secondary-hover: #0b7de3;
            --bg-card: rgba(255, 255, 255, 0.95);
            --shadow: 0 4px 12px rgba(0,0,0,0.2);
            --border-radius: 15px;
        }

        body {
            font-family: 'Kanit', sans-serif;
            background: url('image/bg.png') no-repeat center center fixed;
            background-size: cover;
            margin: 0;
            padding: 0;
            color: #333;
        }
        .container {
            max-width: 650px;
            margin: 50px auto;
            background: var(--bg-card);
            padding: 40px;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            text-align: center;
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1 {
            color: var(--primary-color);
            font-size: 52px;
            margin-bottom: 25px;
            font-weight: 600;
        }
        h2 {
            color: var(--secondary-color);
            font-size: 38px;
            margin-top: 30px;
            margin-bottom: 20px;
            font-weight: 600;
        }
        label {
            font-size: 24px;
            color: #555;
            display: block;
            margin: 15px 0 8px;
            text-align: left;
        }
        input, select {
            width: 100%;
            padding: 12px;
            font-size: 18px;
            margin-bottom: 20px;
            border-radius: 10px;
            border: 1px solid #ccc;
            transition: border-color 0.3s ease;
        }
        input:focus, select:focus {
            border-color: var(--primary-color);
            outline: none;
        }

        .btn-group {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            margin-top: 25px;
        }
        .btn-group button {
            width: 48%;
            margin-bottom: 15px;
            padding: 15px;
        }
        button {
            font-size: 24px;
            padding: 15px 30px;
            border: none;
            border-radius: 12px;
            background-color: var(--button-primary);
            color: white;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
            margin-top: 15px;
            font-weight: 600;
        }
        button:hover {
            transform: translateY(-3px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        .submit-btn:hover {
            background-color: var(--button-hover);
        }
        .category-btn {
            background-color: var(--button-secondary);
            font-size: 20px;
        }
        .category-btn:hover {
            background-color: var(--button-secondary-hover);
        }
        .category-btn.active {
            background-color: var(--button-secondary-hover);
            border: 2px solid white;
            transform: scale(1.05);
        }
        #randomButton {
            background-color: var(--secondary-color);
        }
        #randomButton:hover {
            background-color: #c02d6b;
        }

        #resultContainer {
            margin-top: 40px;
            padding-top: 30px;
            border-top: 2px solid #ddd;
            animation: fadeIn 1s ease-in-out;
        }
        #resultContainer img {
            max-width: 100%;
            height: auto;
            border: 6px solid #f0f0f0;
            border-radius: 20px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.2);
            margin-top: 30px;
        }
        .note {
            color: #d9534f;
            font-size: 16px;
            margin-top: 25px;
            font-style: italic;
        }
        .close-button {
            background-color: #f44336;
        }
        .close-button:hover {
            background-color: #d32f2f;
        }
        .inline-buttons button {
            width: 48%;
            display: inline-block;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>ข้อมูลสุขภาพ</h1>
        <form id="myForm" onsubmit="event.preventDefault(); sendData();">
            <label for="height">ส่วนสูง (ซม.):</label>
            <input type="number" id="height" required>

            <label for="weight">น้ำหนัก (กก.):</label>
            <input type="number" id="weight" required>

         

            <h2>ภาวะสุขภาพพิเศษ</h2>

            <label for="diabetes">เบาหวาน:</label>
            <select id="diabetes" required>
                <option value="">-- โปรดเลือก --</option>
                <option value="yes">มี</option>
                <option value="no">ไม่มี</option>
            </select>

            <label for="hypertension">ความดันโลหิตสูง:</label>
            <select id="hypertension" required>
                <option value="">-- โปรดเลือก --</option>
                <option value="yes">มี</option>
                <option value="no">ไม่มี</option>
            </select>
            
            <button class="submit-btn" type="submit">คำนวณ BMI และสุ่มเมนูที่เหมาะสม</button>
        </form>
        

        <h2>หรือเลือกจากประเภทอาหาร</h2>
        <div class="btn-group">
            <button class="category-btn" onclick="selectCategory('เส้น')">เส้น</button>
            <button class="category-btn" onclick="selectCategory('จานเดียว')">จานเดียว</button>
            <button class="category-btn" onclick="selectCategory('แกง')">แกง</button>
            <button class="category-btn" onclick="selectCategory('ทอด')">ทอด</button>
        </div>
        <button id="randomButton" onclick="sendData(selectedCategory)" style="display: none;">สุ่มเมนู</button>

        <div id="resultContainer"></div>
    </div>
    
   

    <script>
        let selectedCategory = null;

        const diabetesMenuOptions = [
            { name: "ข้าวโจ๊กหมู", image: "image/riceA.png" },
            { name: "ข้าวต้มปลา", image: "image/riceB.png" },
            { name: "ข้าวต้มกุ้ง", image: "image/riceC.png" },
            { name: "ลาบเห็ด", image: "image/riceD.png" },
            { name: "อกไก่ย่าง", image: "image/grilled_chicken.png" },
            { name: "ต้มยำปลา", image: "image/tom_yum_fish.png" },
            { name: "สลัดผัก", image: "image/vegetable_salad.png" }
        ];

        const hypertensionMenuOptions = [
            { name: "แกงจืดเต้าหู้", image: "image/tofu_soup.png" },
            { name: "เต้าหู้ทรงเครื่อง", image: "image/tofu_soup0.png" },
            { name: "สลัดโรลกุ้ง", image: "image/tofu_soup1.png" },
            { name: "ปลานึ่งมะนาว", image: "image/steamed_fish.png" },
            { name: "ผักต้ม", image: "image/boiled_vegetables.png" },
            { name: "สลัดผลไม้", image: "image/fruit_salad.png" }
        ];

        const menuOptionsByBMI = {
            "อ้วนมาก": {
                "เส้น": [
                    { name: "ก๋วยเตี๋ยวหมู/เนื้อ ตุ๋น", image: "image/ObeseJ.png" },
                    { name: "ก๋วยเตี๋ยวต้มยำ", image: "image/thinE.png" }
                ],
                "จานเดียว": [
                    { name: "ลาบหมู", image: "image/Obesea.png" },
                    { name: "กะเพราปลาหมึก", image: "image/Obeseb.png" },
                    { name: "ส้มตำไทย", image: "image/ObeseI.png" }
                ],
                "แกง": [
                    { name: "ต้มแซ่บกระดูกอ่อน", image: "image/ObeseC.png" },
                    { name: "แกงจืดเต้าหู้หมูสับ", image: "image/ObeseF.png" }
                ],
                "ทอด": [
                    { name: "ไก่ย่าง", image: "image/ObeseH.png" }
                ]
            },
            "อ้วน": {
                "เส้น": [
                    { name: "ก๋วยเตี๋ยวลุยสวน", image: "image/tC.png" },
                    { name: "ข้าวมันไก่", image: "image/tF.png" }
                ],
                "จานเดียว": [
                    { name: "ซาชิมิ/ข้าวหน้าปลาดิบ", image: "image/tA.png" },
                    { name: "ลาบไก่", image: "image/tB.png" }
                ],
                "แกง": [
                    { name: "แกงส้มปลา", image: "image/tG.png" },
                    { name: "แกงจืดหมูสับสาหร่าย", image: "image/tH.png" }
                ],
                "ทอด": [
                    { name: "ไก่อบสมุนไพร", image: "image/tE.png" },
                    { name: "ข้าวต้มปลากระพง", image: "image/tD.png" }
                ]
            },
            "มาตรฐาน": {
                "เส้น": [
                    { name: "สปาเก็ตตี้ผัดขี้เมา", image: "image/pl.png" },
                    { name: "ก๋วยเตี๋ยวต้มยำ", image: "image/thinE.png" }
                ],
                "จานเดียว": [
                    { name: "กะเพราไก่ + ไข่ดาว", image: "image/thinA.png" },
                    { name: "ข้าวผัดกุ้งใส่ไข่", image: "image/thinB.png" },
                    { name: "ข้าวผัดผักรวม", image: "image/thinC.png" }
                ],
                "แกง": [
                    { name: "แกงเขียวหวาน", image: "image/thinG.png" }
                ],
                "ทอด": [
                    { name: "ส้มตำไทย/ไก่ย่าง", image: "image/thinF.png" },
                    { name: "ปลาทอด/ผักสด", image: "image/tJ.png" }
                ]
            },
            "ผอม": {
                "เส้น": [
                    { name: "ผัดไทยไข่", image: "image/pC.png" },
                    { name: "ข้าวต้มหมูสับ/กุ้งใส่ขิง", image: "image/pD.png" }
                ],
                "จานเดียว": [
                    { name: "ข้าวคลุกกะปิ + หมูหวาน", image: "image/thA.png" },
                    { name: "ข้าวหมูกระเทียมราดไข่ดาว", image: "image/pB.png" },
                    { name: "ข้าวผัดผักรวมใส่กุ้ง", image: "image/pE.png" }
                ],
                "แกง": [],
                "ทอด": [
                    { name: "สเต็กหมูพริกไทยดำ", image: "image/pG.png" },
                    { name: "ข้าวหน้าไก่ทอด", image: "image/pH.png" },
                    { name: "ข้าวหมูกรอบ", image: "image/pA.png" }
                ]
            },
            "ต่ำกว่าเกณฑ์": {
                "เส้น": [
                    { name: "ข้าวยำปักษ์ใต้", image: "image/swF.png" }
                ],
                "จานเดียว": [
                    { name: "ข้าวผัดกระเพราหมู/ไข่ดาว", image: "image/swA.png" },
                    { name: "ข้าวผัดหมูใส่กุ้ง", image: "image/swB.png" },
                    { name: "ข้าวผัดผักรวมมิตร", image: "image/swC.png" },
                    { name: "ส้มตำ/ไก่ย่าง", image: "image/swD.png" },
                    { name: "ลาบหมู/ไก่", image: "image/swE.png" },
                    { name: "ผัดเผ็ดปลาดุก", image: "image/swH.png" }
                ],
                "แกง": [],
                "ทอด": [
                    { name: "ข้าวหน้าไก่เทอริยากิ", image: "image/swG.png" }
                ]
            }
        };
        
        function getCombinedMenuOptions() {
            const userCustomMenus = JSON.parse(localStorage.getItem('userCustomMenus')) || {};
            const combinedOptions = JSON.parse(JSON.stringify(menuOptionsByBMI));

            for (const bmiStatus in userCustomMenus) {
                if (combinedOptions[bmiStatus]) {
                    for (const category in userCustomMenus[bmiStatus]) {
                        if (!combinedOptions[bmiStatus][category]) {
                            combinedOptions[bmiStatus][category] = [];
                        }
                        combinedOptions[bmiStatus][category] = combinedOptions[bmiStatus][category].concat(userCustomMenus[bmiStatus][category]);
                    }
                }
            }
            return combinedOptions;
        }

        function loadSavedData() {
            // ลบโค้ดส่วนนี้ออกเพื่อไม่ให้ดึงค่าที่เคยบันทึกไว้มาแสดง
            // const savedHeight = localStorage.getItem("userHeight");
            // const savedWeight = localStorage.getItem("userWeight");
            // if (savedHeight) document.getElementById("height").value = savedHeight;
            // if (savedWeight) document.getElementById("weight").value = savedWeight;
        }

        function getBMIStatus(bmi) {
            if (bmi >= 30.0) return { status: "อ้วนมาก", color: "red" };
            if (bmi >= 25.0) return { status: "อ้วน", color: "orange" };
            if (bmi >= 19.0) return { status: "มาตรฐาน", color: "green" };
            if (bmi >= 18.6) return { status: "ผอม", color: "blue" };
            return { status: "ต่ำกว่าเกณฑ์", color: "pink" };
        }

        function getRecommendedMenu(status, diabetes, hypertension, category = null) {
            let avoidFood = "";
            let combinedMenu = [];
            
            const allMenuOptions = getCombinedMenuOptions();

            if (diabetes === "yes" || hypertension === "yes") {
                if (diabetes === "yes") {
                    avoidFood += "⚠️ ผู้ป่วยเบาหวานควรเลี่ยง: น้ำตาล ของหวาน น้ำอัดลม ขนมหวาน<br>";
                    combinedMenu = combinedMenu.concat(diabetesMenuOptions);
                }
                if (hypertension === "yes") {
                    avoidFood += "⚠️ ผู้ป่วยความดันควรเลี่ยง: อาหารเค็มจัด ของหมักดอง อาหารแปรรูป<br>";
                    combinedMenu = combinedMenu.concat(hypertensionMenuOptions);
                }
                if (combinedMenu.length > 0) {
                    const randomIndex = Math.floor(Math.random() * combinedMenu.length);
                    return {
                        menu: "✅ เมนูที่แนะนำสำหรับวันนี้: " + combinedMenu[randomIndex].name,
                        image: combinedMenu[randomIndex].image,
                        avoid: avoidFood,
                        isDisease: true
                    };
                }
            }
            
            let menuList = [];
            if (category && allMenuOptions[status] && allMenuOptions[status][category]) {
                menuList = allMenuOptions[status][category];
            } else if (allMenuOptions[status]) {
                const allCategories = Object.values(allMenuOptions[status]).flat();
                menuList = allCategories;
            }

            if (menuList.length === 0) {
                return {
                    menu: "ไม่พบเมนูสำหรับหมวดหมู่นี้",
                    image: "ไม่มีรูปภาพ",
                    avoid: "",
                    isDisease: false
                };
            }

            const randomIndex = Math.floor(Math.random() * menuList.length);
            const selectedMenu = menuList[randomIndex];

            return {
                menu: "🍛 เมนูแนะนำวันนี้: " + selectedMenu.name,
                image: selectedMenu.image,
                avoid: "",
                isDisease: false
            };
        }

        function sendData(category = null) {
            const height = parseFloat(document.getElementById("height").value);
            const weight = parseFloat(document.getElementById("weight").value);
            const diabetes = document.getElementById("diabetes").value;
            const hypertension = document.getElementById("hypertension").value;

            localStorage.setItem("userHeight", height);
            localStorage.setItem("userWeight", weight);

            if (height <= 0 || weight <= 0 || isNaN(height) || isNaN(weight)) {
                alert("กรุณาใส่ข้อมูลส่วนสูงและน้ำหนักที่ถูกต้อง");
                return;
            }

            const heightM = height / 100;
            const BMI = weight / (heightM * heightM);
            const { status, color } = getBMIStatus(BMI);

            const recommended = getRecommendedMenu(status, diabetes, hypertension, category);

            const record = {
                date: new Date().toLocaleString("th-TH"),
                bmi: BMI.toFixed(2),
                status: status,
                menu: recommended.menu.replace("✅ เมนูที่แนะนำสำหรับวันนี้: ", "").replace("🍛 เมนูแนะนำวันนี้: ", ""),
                image: recommended.image
            };
            let history = JSON.parse(localStorage.getItem("menuHistory")) || [];
            history.unshift(record);
            localStorage.setItem("menuHistory", JSON.stringify(history));

            displayResult(BMI, status, color, recommended);
        }
        
        function selectCategory(category) {
            selectedCategory = category;
            const buttons = document.querySelectorAll('.category-btn');
            buttons.forEach(btn => btn.classList.remove('active'));
            document.querySelector(`.category-btn[onclick="selectCategory('${category}')"]`).classList.add('active');
            document.getElementById("randomButton").textContent = `สุ่มเมนูหมวด "${category}"`;
            document.getElementById("randomButton").style.display = "block";
        }

        function displayResult(bmi, status, color, recommended) {
            const resultDiv = document.getElementById("resultContainer");
            resultDiv.innerHTML = `
                <h1>ดัชนีมวลกาย (BMI): ${bmi.toFixed(2)}</h1>
                <h2 style='color:${color};'>สถานะน้ำหนัก: ${status}</h2>
                ${recommended.avoid ? `<p style='text-align: left;'>${recommended.avoid}</p>` : ''}
                <h2>${recommended.menu}</h2>
                <div>
                    <img src='${recommended.image}' width='360' alt='เมนูอาหาร'>
                </div>
                <p class='note'>⚠️ หมายเหตุ: คำแนะนำนี้เป็นข้อมูลเบื้องต้น ไม่สามารถแทนคำแนะนำทางการแพทย์ได้ หากมีโรคประจำตัวควรปรึกษาแพทย์หรือนักโภชนาการ</p>
                <div class="inline-buttons">
                    <button onclick="window.open('history.html', '_blank', 'width=700,height=600,scrollbars=yes')" style="background-color:#04aa6a;">ดูประวัติ</button>
                   
                </div>
            `;
        }

        window.onload = loadSavedData;
    </script>
</body>
</html>
