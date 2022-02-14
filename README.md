# Anomaly-Detection-in-Cellular-Networks-based-on-Network-Function-KPI

# 摘要
隨著互聯網的高速發展，網路服務已經快速深入到社會當中，人們大量上網從事購物、付款、娛樂等等活動，因此保障網路的穩定性非常重要。
網路服務的穩定性主要靠維運人員監控各式各樣的關鍵性能指標(Key Performance Indicators，簡稱KPI)來判斷網路是否穩定。由於KPI發生異常，往往代表著與其相對的應用或服務發生了問題，若無法在異常發生前將其識別且進行修復，會導致要求呼叫失敗、網路延遲等故障，對全網的服務質量帶來重大的負面影響， 有時甚至等到用戶投訴時才發現異常情況，將會使用戶體驗大大受損。
# 簡介
KPI異常檢測指的是透過演算法分析KPI的時間序列數據，並標記網路在何時發生異常，然後利用其時間序列的規律性進行異常預測，如此一來能夠幫助維運人員提前發現未知風險，降低網路因異常帶來的損失。KPI異常預測有以下難點存在：
\n
(1) 在實際網路服務場景中，異常發生的頻率相對很低，因此可供分析的異常樣本非常少。
\n
(2) 由於核心網網元數據多，並且會不斷更新升級，從而導致異常種類的多樣性。
\n
(3) KPI曲線的多樣性，如週期型或波動型等等。因為這些難點，導致大量異常誤報和漏報的存在，如何設計一個高效且具有較強泛化能力的異常檢測模型即是一大挑戰。
本研究的實驗數據來自2021華為某次學習賽提供之某網路營運商之部分網元的KPI真實數據，數據採樣間隔為一小時，我們根據歷史一個月的數據訓練各種模型並預測隨後一周內KPI中的異常情況。本文從多維度特徵
