---
title: "選擇正確的緩動"
description: "為您的專案選擇適當的緩動，無論是緩入、緩出或兩者。 也許甚至帶點彈性，以求趣味效果！"
updated_on: 2014-10-21
key-takeaways:
  code:
    - 針對 UI 元素使用緩出動畫，是非常不錯但帶敏捷感的緩和效果。
    - 確定要用上動畫持續時間；緩出和緩入應該介於 200ms - 500ms 之間，而彈跳和彈性緩動應設定在較長的 800ms - 1200ms 持續時間。

---
<p class="intro">
  在討論了動畫中緩入的各種選項之後，您在專案中應該使用哪一種，以及您動畫應該使用哪一種持續時間？
</p>

{% include shared/takeaway.liquid list=page.key-takeaways.code %}

一般而言 **緩出** 會是正確的決定，當然也是個好的預設設定。 它會快速開始、給您動畫反應快的操作感 (這當然很受歡迎)，但結束帶有不錯的放緩效果。

除了 CSS 中以 `ease-out` 關鍵字指定的那一個，目前已有一組知名的緩出方程式，以其「侵略性」分類在同一組。 至於超級敏捷的緩出效果，請考慮 [Quintic 緩出](http://easings.net/#easeOutQuint)。

<img src="imgs/quintic-ease-out-markers.png" alt=" Quintic 緩出動畫曲線" style="max-width: 300px"/>

{% link_sample _code/box-move-quintic-ease-out.html %}參閱 Quintic 緩出動畫。{% endlink_sample %}

尤其是彈跳或彈性緩動等其他緩動方程式，應節制使用，而且只有在適合於您專案時才使用。 還有幾件事情，會像刺耳的動畫一般讓使用者非常出戲。 如果您的專案並不快樂有趣，那麼不要讓 UI 元素四處發出啵嚶聲！反之，如果您正在製作應該要輕鬆有趣的網站，那就當然可以設計彈跳效果！

玩弄一下緩動效果，看看哪些符合您專案的特性，並以此為起點。 帶示範的緩動類型之完整清單，可在 [easings.net](http://easings.net)找到。

## 選擇正確的動畫持續時間

重要的是要讓新增到您專案的任何動畫，具有正確的持續時間。 太短會讓動畫會感覺侵略性且急劇；太長會讓動畫礙事又討厭。

* **緩出：大約 200ms - 500ms**。 這讓眼睛有機會看到動畫，但又不感到礙事。
* **緩入：大約 200ms - 500ms**。 請記住，它在結尾將會搖晃，任何計時變更都無法柔化此操作感。
* **彈跳或彈性效果：大約 800ms - 1200ms**。 您需要允許一些時間，讓彈性或彈跳效果平靜下來。 若無這段額外時間，動畫的彈性彈跳部分對眼睛而言，將會非常具侵略性和令人不快。

當然以上這些都只是基本方針。 以您自己的緩動進行實驗，並選擇適合您專案的設計。


