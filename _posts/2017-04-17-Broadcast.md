---
layout: default
permalink: Android_Broadcast
---

> {{ page.date | date_to_string }}

## Android Broadcast

### 广播接收类的两种注册方法

#### 静态注册

	<receiver android:name=".MainActivity$broadcastReceiver">
            <intent-filter>
                <action android:name="MainActivity"/>
            </intent-filter>
    </receiver>

#### 动态注册

	private broadcastReceiver receiver;
	IntentFilter filter = new IntentFilter();
	filter.addAction("MainActivity");
	receiver = new broadcastReceiver();
	registerReceiver(receiver, filter);


#### PS

* 当广播为内部类时，必须使其为静态类才能使用静态注册的方法	




<br />
<br />
<br />


[back](../)