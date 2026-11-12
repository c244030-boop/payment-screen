# payment-screen<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport"
        content="width=device-width, initial-scale=1, maximum-scale=1">
  <title>お支払い</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      background: #f4f6f8;
      color: #202124;
      font-family:
        -apple-system, BlinkMacSystemFont,
        "Hiragino Sans", "Yu Gothic", sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px;
    }

    .screen {
      width: 100%;
      max-width: 420px;
      background: #ffffff;
      border-radius: 24px;
      padding: 28px 22px;
      box-shadow: 0 8px 28px rgba(0, 0, 0, 0.12);
    }

    .title {
      text-align: center;
      font-size: 18px;
      font-weight: 700;
      margin-bottom: 28px;
    }

    .label {
      color: #687078;
      font-size: 14px;
      text-align: center;
    }

    .amount {
      font-size: 42px;
      font-weight: 800;
      text-align: center;
      margin: 6px 0 30px;
    }

    .info {
      background: #f3f7fa;
      border-radius: 14px;
      padding: 16px;
      margin-bottom: 22px;
    }

    .row {
      display: flex;
      justify-content: space-between;
      gap: 16px;
      margin: 8px 0;
      font-size: 15px;
    }

    .row strong {
      text-align: right;
    }

    button {
      width: 100%;
      border: 0;
      border-radius: 14px;
      background: #087f8c;
      color: white;
      padding: 16px;
      font-size: 17px;
      font-weight: 700;
      cursor: pointer;
    }

    button:active {
      transform: scale(0.99);
    }

    .complete {
      display: none;
      text-align: center;
    }

    .check {
      width: 68px;
      height: 68px;
      margin: 0 auto 20px;
      border-radius: 50%;
      background: #16875b;
      color: white;
      font-size: 42px;
      line-height: 68px;
      font-weight: 700;
    }

    .complete-title {
      font-size: 22px;
      font-weight: 800;
      margin-bottom: 24px;
    }

    .complete-note {
      margin-top: 18px;
      color: #59636c;
      line-height: 1.7;
    }
  </style>
</head>

<body>
  <main class="screen">

    <section id="confirm">
      <div class="title">お支払い内容の確認</div>

      <div class="label">今回のお支払い</div>
      <div class="amount" id="amountConfirm">750円</div>

      <div class="info">
        <div class="row">
          <span>支払方法</span>
          <strong id="methodConfirm">チャージ残高</strong>
        </div>

        <div class="row" id="balanceRow">
          <span>決済前残高</span>
          <strong id="balanceConfirm">1,000円</strong>
        </div>

        <div class="row" id="dateRow" style="display:none;">
          <span>支払日</span>
          <strong>翌月27日</strong>
        </div>
      </div>

      <button type="button" id="payButton">
        確認して支払う
      </button>
    </section>

    <section id="complete" class="complete" aria-live="polite">
      <div class="check">✓</div>
      <div class="complete-title">支払いが完了しました</div>

      <div class="label">お支払い金額</div>
      <div class="amount" id="amountComplete">750円</div>

      <div class="info">
        <div class="row">
          <span id="resultLabel">チャージ残高</span>
          <strong id="resultValue">250円</strong>
        </div>
      </div>

      <div class="complete-note" id="completeNote"></div>
    </section>

  </main>

  <script>
    const params = new URLSearchParams(window.location.search);

    const amount = Math.max(
      0,
      Number.parseInt(params.get("amount") || "750", 10)
    );

    const balance = Math.max(
      0,
      Number.parseInt(params.get("balance") || "1000", 10)
    );

    const type =
      params.get("type") === "postpaid"
        ? "postpaid"
        : "prepaid";

    const yen = value => `${value.toLocaleString("ja-JP")}円`;

    document.getElementById("amountConfirm").textContent = yen(amount);
    document.getElementById("amountComplete").textContent = yen(amount);

    if (type === "prepaid") {
      document.getElementById("methodConfirm").textContent =
        "チャージ残高";

      document.getElementById("balanceConfirm").textContent =
        yen(balance);

      document.getElementById("dateRow").style.display = "none";

      document.getElementById("resultLabel").textContent =
        "決済後残高";

      document.getElementById("resultValue").textContent =
        yen(Math.max(0, balance - amount));

      document.getElementById("completeNote").textContent =
        "チャージ残高から代金が差し引かれました。";
    } else {
      document.getElementById("methodConfirm").textContent =
        "あと払い";

      document.getElementById("balanceRow").style.display = "none";
      document.getElementById("dateRow").style.display = "flex";

      document.getElementById("resultLabel").textContent =
        "支払日";

      document.getElementById("resultValue").textContent =
        "翌月27日";

      document.getElementById("completeNote").textContent =
        `${yen(amount)}は翌月27日に登録口座から引き落とされます。`;
    }

    document
      .getElementById("payButton")
      .addEventListener("click", () => {
        document.getElementById("confirm").style.display = "none";
        document.getElementById("complete").style.display = "block";
      });
  </script>
</body>
</html>
