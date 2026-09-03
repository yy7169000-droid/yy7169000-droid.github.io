<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>테런 염색코드 변환기</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --accent-color: #3498db;
            --bg-color: #f8f9fa;
            --card-bg: #ffffff;
        }
        body {
            font-family: 'Pretendard', 'Malgun Gothic', sans-serif;
            background-color: var(--bg-color);
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
        }
        .container {
            background-color: var(--card-bg);
            border-radius: 12px;
            box-shadow: 0 8px 24px rgba(0,0,0,0.08);
            max-width: 900px;
            width: 100%;
            overflow: hidden;
        }
        .header {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 20px;
        }
        .header h1 {
            margin: 0;
            font-size: 22px;
        }
        .color-slots {
            display: flex;
            padding: 25px;
            gap: 20px;
        }
        .slot {
            flex: 1;
            background: #fdfdfd;
            border: 1px solid #e1e4e8;
            border-radius: 8px;
            padding: 15px;
            display: flex;
            flex-direction: column;
            gap: 12px;
        }
        .slot-title {
            text-align: center;
            font-weight: 700;
            color: var(--primary-color);
            font-size: 15px;
            border-bottom: 2px solid #f1f2f6;
            padding-bottom: 8px;
        }
        .input-box input {
            width: 100%;
            box-sizing: border-box;
            padding: 10px;
            font-size: 14px;
            text-align: center;
            border: 2px dashed #b2bec3;
            border-radius: 6px;
            background-color: #fbfcff;
            outline: none;
        }
        .input-box input:focus {
            border-color: var(--accent-color);
        }
        .result-box {
            display: flex;
            justify-content: space-between;
            background-color: #f1f2f6;
            border-radius: 6px;
