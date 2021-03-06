---
last_modified: 2015/03/31
translation_status: complete
language: ja
title: Datadogが提供するサービスの概要
kind: documentation
sidebar:
  nav:
    - header: Datadogのサービスについて
    - text: Integrations 機能
      href: "#integrations"
    - text: Infrastructure 機能
      href: "#infrastructure"
    - text: Events 機能
      href: "#events"
    - text: dashboards 機能
      href: "#dashboards"
    - text: アラート機能
      href: "#alerting"
---


<!-- So, you've just finished [installing](/guides/basic_agent_usage/) the Datadog
Agent, or maybe you're just curious about [what (else) Datadog can do for you](http://www.datadoghq.com/product/).
This document gives a high level overview of Datadog's capabilities and how
it can help you bring your infrastructure to heel. -->

Datadog Agentの[インストール](/ja/guides/basic_agent_usage/)は、無事終了しましたか。もしかしたら、[Datadogが提供するサービス](http://www.datadoghq.com/product/)に興味を持っていただいたばかりかもしれませんね。

このドキュメントでは、**Datadogの各機能**と**それらの有要性**を解説します。


<!-- <h2 id="integrations">Integrations</h2>

<img src="/static/images/integrations.png" style="width:100%; border:1px solid #777777"/>

<ul>
<li>60+ integrations <a target="_blank" href="http://www.datadoghq.com/integrations/">officially listed</a>,
always adding more.</li>
<li>Custom integrations are available <a target="_blank" href="http://docs.datadoghq.com/api/">via our API</a>,
many documented by our active user community.</li>
<li>The Agent is <a target="_blank" href="https://github.com/DataDog/dd-agent/">open source</a> and you
can instrument your own if you'd like.</li>
<li>Once integrations have been configured, data living in a datacenter or
in an online service is treated the same throughout Datadog.</li>
</ul> -->

<h2 id="integrations">Integrations 機能</h2>

<img src="/static/images/integrations.png" style="width:100%; border:1px solid #777777"/>

<ul>
<li>60以上のIntegrations を公式に<a target="_blank" href="http://www.datadoghq.com/integrations/">公開中</a>です。Integrationsは随時追加される予定です。</li>
<li>カスタム Integrationsは、<a target="_blank" href="/ja/api/">Datadog API</a>を介し開発することができます。これらのAPIは、活発なユーザーコミュニティによってドキュメント化が進められています。</li>
<li><a target="_blank" href="https://github.com/DataDog/dd-agent/">Datadog Agent</a> はオープンソースです。 必要に応じて独自に改造することもできます。</li>
<li>Integrationの設定が完了すればデータセンターやオンラインサービス等から転送したデータもDatadogを介し同じように取り扱うことができます。</li>
</ul>


<!-- <h2 id="infrastructure">Infrastructures</h2>

<img src="/static/images/infrastructure.png" style="width:100%; border:1px solid #777777"/>

<ul>
<li>All machines show up in the infrastructure overview</li>
<li>Here you can see the tags applied to each machine; as they're assigned to
perform certain roles, tagging allows you to indicate machines have
a certain purpose</li>
<li>We do as much as possible to automatically categorize your servers
for you, to create structure in your infrastructure with as little
work as possible (unlike explicitly creating all your clusters).
Thus if a new machine is tagged, you can immediately see the stats
for that machine based on what was previously set up for that tag.</li>
<li>For more on tagging, please see <a target="_blank" href="/faq/#tagging">here</a>.

</li>

</ul> -->

<h2 id="infrastructure">Infrastructure 機能</h2>

<img src="/static/images/infrastructure.png" style="width:100%; border:1px solid #777777"/>

<ul>
<li>全てのホストは、Infrastructureのページに表示されます。</li>
<li>上の図では、各種の役割を与えられたホストに適用されたタグを見ることができます。タグを付与することによって各ホストがどのような目的で利用されているか識別することができます。</li>
<li>Datadogでは、インフラ全体の構造を最小限の努力で表現できるように、ホストをできる限り自動的に分類するようにしています。明示的に、すべてのクラスタの作成する必要はありません。従って新しいホストにタグが付与されると、以前にそのタグ用に設定した内容にしたがい直ちにステータスを見ることができるように成ります。</li>
<li>タグ設定の詳細は、<a target="_blank" href="/ja/faq/#tagging">"FAQ:タグの詳細"</a>をご参照ください。</li>

</ul>


<!-- <h2 id="events">Events</h2>

<img src="/static/images/event_stream.png" style="width:100%; border:1px solid #777777"/>

The Event Stream is based on the same conventions as a blog:
<ul>
<li>Every event in the stream can be commented on.</li>
<li>Great for distributed <a target="_blank" href="/faq/#team">teams</a> and maintaining the focus of an investigation</li>
<li>You can <a target="_blank" href="https://www.datadoghq.com/2014/05/filter-datadog-events-stream-pinpoint-events-infrastructure/">filter</a>
by: user, source, tag, host, status, priority, incident</li>
</ul>

<img src="/static/images/event_stream_post_incident_history.png" style="width:100%; border:1px solid #777777"/>

For each incident users can:
<ul>
<li>Claim it</li>
<li>Increase/decrease priority</li>
<li>Comment</li>
<li>See similar incidents </li>
<li><a target="_blank" href="/faq/#notify">@ notify team members</a>, who receive an email</li>
<li>@support to ask for assistance</li>
</ul>

<img src="/static/images/event_stream_claim.png" style="width:100%; border:1px solid #777777"/>
 -->

<h2 id="events">Events 機能</h2>

<img src="/static/images/event_stream.png" style="width:100%; border:1px solid #777777"/>

Eventの掲載は、ブログと同じ規則に基づいています:

<ul>
<li>ストリーム内のすべてのEventにはコメントを付けることができます。</li>
<li>分散した<a target="_blank" href="/ja/faq/#team">チーム</a>や、問題の調査時に問題点をフォーカスするのに便利です。</li>
<li>by: user, source, tag, host, status, priority, incident 等の項目で、<a target="_blank" href="https://www.datadoghq.com/2014/05/filter-datadog-events-stream-pinpoint-events-infrastructure/">フィルタリング</a>することができます。</li>
</ul>

<img src="/static/images/event_stream_post_incident_history.png" style="width:100%; border:1px solid #777777"/>

ユーザは、インシデント(出来事)に対して次の操作ができます:
<ul>
<li>問題の提案</li>
<li>プライオリティの変更(上げる/下げる)</li>
<li>コメントの追加</li>
<li>同様なインシデントの閲覧</li>
<li><a target="_blank" href="/ja/faq/#notify">@ notify</a>を使ったチームメンバーへの通知やemail送信</li>
<li>@support でのサポートの要請</li>
</ul>

<img src="/static/images/event_stream_claim.png" style="width:100%; border:1px solid #777777"/>


<!-- <h2 id="dashboards">dashboards</h2>

<img src="/static/images/dashboard_events.png" style="width:100%; border:1px solid #777777"/>

Dashboards contain <a target="_blank" href="/graphing/">graphs</a> with real-time performance metrics
<ul>
<li>Synchronous mousing across all graphs in a dashboard.	</li>
<li>Vertical bars are events in the context of the metric.</li>
<li>Click & drag on a graph to zoom-in on a particular time-frame.</li>
<li>As you hover over the graph the event stream moves with you.</li>
<li>Display by zone, host, or total usage.</li>
<li>We expose the JSON editor of the graph allowing for <a target="_blank" href="http://docs.datadoghq.com/graphing/#functions">arithmetic</a> and
<a target="_blank" href="https://www.datadoghq.com/2014/04/rank-filter-performance-monitoring-metrics-top-function/">functions</a> to be applied to metrics.</li>
<li>Share a graph snapshot that will appear in the stream; clicking on
that snapshot returns you to the original dashboard (via the camera in the upper right of a graph).</li>
<li>Graphs can be embedded in an iframe, giving a 3rd party a live graph
without access to your data or any other information (via the cog in the upper right of a graph).</li>
</ul> -->

<h2 id="dashboards">ダッシュボード機能</h2>

<img src="/static/images/dashboard_events.png" style="width:100%; border:1px solid #777777"/>

ダッシュボードには、<a target="_blank" href="/ja/graphing/">グラフ化</a>されたパフォーマンスメトリクスがリアルタイムに表示されます。
<ul>
<li>ダッシュボード内の全てのグラフは、マウスで操作できます。</li>
<li>グラフ内のビンクの縦の線は、Eventの発生を表しています。</li>
<li>グラフ上で"Click & drag"することによって、時間軸を変更することができます。</li>
<li>グラフ上でカーソルを移動することによって、Eventストリームの表示も該当箇所へ自動的に移動していきます。</li>
<li>zone, host, total usageで、表示することができます。</li>
<li>グラフ内に表示するメトリクスの<a target="_blank" href="/ja/graphing/#functions">計算</a>や<a target="_blank" href="https://www.datadoghq.com/2014/04/rank-filter-performance-monitoring-metrics-top-function/">統計</a>を可能にするために、JSON editorを画面上に設置しています。</li>
<li>グラフのスナップショットをEventストリームで共有することができます。Eventストリームに掲載されたスナップショットを"Click"すると、そのグラフが表示されているダッシュボードに移動することができます。(グラフ右上のカメラマークから)</li>
<li>グラフは、iframeに挿入することができます。この機能を使い、基礎データや他の情報を隠蔽したまま、第３者に<!-- ライブな -->グラフを公開することができます。(グラフ右上の歯車マークから)</li>
</ul>


<!-- <h2 id="alerting">Alerting</h2>
<img src="/static/images/alert.png" style="width:100%; border:1px solid #777777"/>

[Alerting](/guides/alerting/) gives you the ability to be notified if the aggregate of a specific
metric is above or below a certain threshold:
<ul>
<li>Across your entire infrastructure</li>
<li>Per machine (average, max, min, or sum) </li>
<li>Applies to any metric you want, revenue: data center temperature, etc.</li>
<li>Multi alerts (by device, host, etc.)</li>
<li>Set alert notification message, including @ capabilities</li>
</ul>

<img src="/static/images/alert_setup.png" style="width:100%; border:1px solid #777777"/>

Does the data have to be pushed to Datadog?
<ol>
Currently, yes:
<li>All integrations we have get data flowing almost automatically after
launching the Agent (intial reporting may take a few minutes, but not longer than 10).</li>
<li>If you have custom metrics, you can indicate specifically where
to pull the data from.</li>
</ol> -->

<h2 id="alerting">アラート機能</h2>
<img src="/static/images/alert.png" style="width:100%; border:1px solid #777777"/>

[アラート機能](/ja/guides/alerting/)によって、特定のメトリクスの集計がしきい値を超えた場合に通知する機能を実現することができます:
<ul>
<li>インフラ全体のメトリクスのaverage, max, min, or sumを基に</li>
<li>ホスト毎のメトリクスのaverage, max, min, or sumを基に</li>
<li>指定できるメトリクスなら全てOK。例: 売上情報, データーセンターの温度, など</li>
<li>同一条件による、別デバイスや別ホストに股がったアラート機能 (by device, host, etc.)</li>
<li>"@"機能によるグループ毎の通知設定</li>
</ul>

<img src="/static/images/alert_setup.png" style="width:100%; border:1px solid #777777"/>

アラート機能のためのデータは、Datadogに送信する必要がありますか?
<ol>
はい、必要です。:
<li>Datadogで公開しているIntegrationsは、Datadog Agent を起動することによって、自動的にデータを送信するように成っています。(初回のデータ送信に関しては、数分の時間を要します。但し、10分以上になることはありません。)</li>
<li>カスタムメトリクスがある場合は、データの収集先情報を特別に指定することができます。</li>
</ol>
