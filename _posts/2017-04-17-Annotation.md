---
layout: default
permalink: Android_Annotation
---

> {{ page.date | date_to_string }}

## Android Annotation

### 利用注释来设置可选函数值

	@IntDef({Order_cycle, Single_repetition, shuffle})	//其中的参数为待选值
    @Retention(RetentionPolicy.SOURCE)
    public @interface PlayMode {}

	//在方法参数处设置如下
	public void changePlayMode(@PlayMode int playMode) {
          
    }


<br />
<br />
<br />


[back](../)