Android Auto Scroll Loop View Pager
=======================

Combine from follow libraray:

1. Trinea/[AutoScrollViewPager](https://github.com/Trinea/android-auto-scroll-view-pager)

- ViewPager which can auto scroll, cycle.

- ViewPager which can be slided normal in parent ViewPager.

![android-auto-scroll-view-pager](http://farm3.staticflickr.com/2843/12805132475_e595664a81_o.gif)

2. imbryk/[LoopingViewPager](https://github.com/imbryk/LoopingViewPager)

An android ViewPager extension allowing infinite scrolling.


## Usage
- include the jar file and android-support-v4.jar, use

``` xml
<io.github.neutra.android.autoscrollloopviewpager.AutoScrollLoopViewPager
	android:id="@+id/view_pager"
	android:layout_width="match_parent"
	android:layout_height="wrap_content" />
```
replace
``` xml
<android.support.v4.view.ViewPager
	android:id="@+id/view_pager"
	android:layout_width="match_parent"
	android:layout_height="wrap_content" />
```
- `startAutoScroll()` start auto scroll, delay time is `getInterval()`.
- `startAutoScroll(int)` start auto scroll delayed.
- `stopAutoScroll()` stop auto scroll.

## Setting
- `setInterval(long)` set auto scroll time in milliseconds, default is `DEFAULT_INTERVAL`.
- `setDirection(int)` set auto scroll direction, default is `RIGHT`.
- `setScrollDurationFactor(double)` set the factor by which the duration of sliding animation will change.
- `setStopScrollWhenTouch(boolean)` set whether stop auto scroll when touching, default is true.
- You may need [ViewPagerIndicator](https://github.com/JakeWharton/Android-ViewPagerIndicator) to implement indicator. 
```

## License
