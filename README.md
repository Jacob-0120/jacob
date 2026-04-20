<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>chang ching fu</title>
    <style>
        /* --- 表格的樣式設定 --- */
        table {
            border-collapse: collapse; /* 讓表格的雙線邊框合併成單線 */
            width: 250px;
            text-align: left;
            margin: 20px; /* 稍微推開邊界比較好看 */
        }

        th, td {
            border: 1px solid black; /* 設定黑色邊框 */
            padding: 10px;
        }

        th {
            background-color: gray; /* 表頭設定為灰色背景 */
            color: white;           /* 表頭文字設為白色 */
        }

        /* 使用 :nth-child(odd) 來選取 tbody 裡的奇數列 (第1、3行) 並設定為黃色 */
        tbody tr:nth-child(odd) {
            background-color: yellow;
        }

        /* --- 右上角浮動區塊的樣式設定 --- */
        .fixed-box {
            position: fixed;         /* 關鍵：設定為固定定位 */
            top: 50px;               /* 距離視窗頂部 50px */
            right: 50px;             /* 距離視窗右側 50px */
            border: 3px solid #6b9e23; /* 設定綠色粗邊框 */
            padding: 10px;
            width: 150px;
            background-color: white; /* 確保背景是白色，才不會透明疊到其他東西 */
        }
    </style>
</head>
<body>

    <table>
        <thead>
            <tr>
                <th>Firstname</th>
                <th>Lastname</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>1</td>
            </tr>
            <tr>
                <td>2</td>
                <td>2</td>
            </tr>
            <tr>
                <td>3</td>
                <td>3</td>
            </tr>
        </tbody>
    </table>

    <div class="fixed-box">
        This div element has position: fixed;
    </div>

</body>
</html>
