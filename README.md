Malikye Wallace
mww180002


# Part 0 Output

r0 := @this: a1.HelloThread$TestThread
specialinvoke r0.<java.lang.Thread: void <init>()>()
return
<a1.HelloThread: int x> = 1
return
r0 := @this: a1.HelloThread
specialinvoke r0.<java.lang.Object: void <init>()>()
return
r0 := @parameter0: java.lang.String[]
$r2 = new a1.HelloThread$TestThread
specialinvoke $r2.<a1.HelloThread$TestThread: void <init>()>()
r0 := @this: a1.HelloThread$TestThread
virtualinvoke $r2.<a1.HelloThread$TestThread: void start()>()
$i3 = $r2.<a1.HelloThread$TestThread: int y>
$i1 = <a1.HelloThread: int x>
$i2 = 1 / $i1
i0 = $i3 + $i2
$r3 = <java.lang.System: java.io.PrintStream out>
<a1.HelloThread: int x> = 0
$i0 = r0.<a1.HelloThread$TestThread: int y>
$i1 = $i0 + 1
r0.<a1.HelloThread$TestThread: int y> = $i1
return
virtualinvoke $r3.<java.io.PrintStream: void println(int)>(i0)
return

## Part 1

The given code appears to produce valid output defining all dominators for each statement when compared to a handdrawn control flow diagram.

r0 := @this: a1.GCD is dominated by r0 := @this: a1.GCD
specialinvoke r0.<java.lang.Object: void <init>()>() is dominated by r0 := @this: a1.GCD
specialinvoke r0.<java.lang.Object: void <init>()>() is dominated by specialinvoke r0.<java.lang.Object: void <init>()>()
return is dominated by r0 := @this: a1.GCD
return is dominated by specialinvoke r0.<java.lang.Object: void <init>()>()
return is dominated by return
r0 := @parameter0: java.lang.String[] is dominated by r0 := @parameter0: java.lang.String[]
$i2 = lengthof r0 is dominated by r0 := @parameter0: java.lang.String[]
$i2 = lengthof r0 is dominated by $i2 = lengthof r0
if $i2 >= 2 goto $r1 = r0[0] is dominated by r0 := @parameter0: java.lang.String[]
if $i2 >= 2 goto $r1 = r0[0] is dominated by $i2 = lengthof r0
if $i2 >= 2 goto $r1 = r0[0] is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r11 = <java.lang.System: java.io.PrintStream err> is dominated by r0 := @parameter0: java.lang.String[]
$r11 = <java.lang.System: java.io.PrintStream err> is dominated by $i2 = lengthof r0
$r11 = <java.lang.System: java.io.PrintStream err> is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r11 = <java.lang.System: java.io.PrintStream err> is dominated by $r11 = <java.lang.System: java.io.PrintStream err>
virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267") is dominated by r0 := @parameter0: java.lang.String[]
virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267") is dominated by $i2 = lengthof r0
virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267") is dominated by if $i2 >= 2 goto $r1 = r0[0]
virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267") is dominated by $r11 = <java.lang.System: java.io.PrintStream err>
virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267") is dominated by virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267")
return is dominated by r0 := @parameter0: java.lang.String[]
return is dominated by $i2 = lengthof r0
return is dominated by if $i2 >= 2 goto $r1 = r0[0]
return is dominated by $r11 = <java.lang.System: java.io.PrintStream err>
return is dominated by virtualinvoke $r11.<java.io.PrintStream: void println(java.lang.String)>("java GCD int1 int2\nExample: java GCD 876 267")
return is dominated by return
$r1 = r0[0] is dominated by r0 := @parameter0: java.lang.String[]
$r1 = r0[0] is dominated by $i2 = lengthof r0
$r1 = r0[0] is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r1 = r0[0] is dominated by $r1 = r0[0]
i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1) is dominated by r0 := @parameter0: java.lang.String[]
i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1) is dominated by $i2 = lengthof r0
i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1) is dominated by if $i2 >= 2 goto $r1 = r0[0]
i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1) is dominated by $r1 = r0[0]
i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r2 = r0[1] is dominated by r0 := @parameter0: java.lang.String[]
$r2 = r0[1] is dominated by $i2 = lengthof r0
$r2 = r0[1] is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r2 = r0[1] is dominated by $r1 = r0[0]
$r2 = r0[1] is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r2 = r0[1] is dominated by $r2 = r0[1]
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by r0 := @parameter0: java.lang.String[]
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by $i2 = lengthof r0
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by if $i2 >= 2 goto $r1 = r0[0]
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by $r1 = r0[0]
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by $r2 = r0[1]
i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2) is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by r0 := @parameter0: java.lang.String[]
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by $i2 = lengthof r0
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by $r1 = r0[0]
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by $r2 = r0[1]
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r4 = <java.lang.System: java.io.PrintStream out> is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r3 = new java.lang.StringBuilder is dominated by r0 := @parameter0: java.lang.String[]
$r3 = new java.lang.StringBuilder is dominated by $i2 = lengthof r0
$r3 = new java.lang.StringBuilder is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r3 = new java.lang.StringBuilder is dominated by $r1 = r0[0]
$r3 = new java.lang.StringBuilder is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r3 = new java.lang.StringBuilder is dominated by $r2 = r0[1]
$r3 = new java.lang.StringBuilder is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r3 = new java.lang.StringBuilder is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r3 = new java.lang.StringBuilder is dominated by $r3 = new java.lang.StringBuilder
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by r0 := @parameter0: java.lang.String[]
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by $i2 = lengthof r0
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by if $i2 >= 2 goto $r1 = r0[0]
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by $r1 = r0[0]
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by $r2 = r0[1]
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by $r3 = new java.lang.StringBuilder
specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(") is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by r0 := @parameter0: java.lang.String[]
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by $i2 = lengthof r0
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by $r1 = r0[0]
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by $r2 = r0[1]
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by $r3 = new java.lang.StringBuilder
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0) is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by r0 := @parameter0: java.lang.String[]
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $i2 = lengthof r0
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $r1 = r0[0]
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $r2 = r0[1]
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $r3 = new java.lang.StringBuilder
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ") is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by r0 := @parameter0: java.lang.String[]
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $i2 = lengthof r0
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r1 = r0[0]
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r2 = r0[1]
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r3 = new java.lang.StringBuilder
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
$r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1) is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by r0 := @parameter0: java.lang.String[]
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $i2 = lengthof r0
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r1 = r0[0]
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r2 = r0[1]
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r3 = new java.lang.StringBuilder
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
$r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ") is dominated by $r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ")
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by r0 := @parameter0: java.lang.String[]
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $i2 = lengthof r0
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by if $i2 >= 2 goto $r1 = r0[0]
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r1 = r0[0]
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r2 = r0[1]
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r3 = new java.lang.StringBuilder
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ")
$i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1) is dominated by $i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1)
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by r0 := @parameter0: java.lang.String[]
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $i2 = lengthof r0
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r1 = r0[0]
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r2 = r0[1]
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r3 = new java.lang.StringBuilder
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ")
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1)
$r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3) is dominated by $r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by r0 := @parameter0: java.lang.String[]
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $i2 = lengthof r0
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by if $i2 >= 2 goto $r1 = r0[0]
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r1 = r0[0]
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r2 = r0[1]
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r3 = new java.lang.StringBuilder
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ")
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3)
$r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>() is dominated by $r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>()
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by r0 := @parameter0: java.lang.String[]
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $i2 = lengthof r0
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by if $i2 >= 2 goto $r1 = r0[0]
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r1 = r0[0]
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r2 = r0[1]
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r3 = new java.lang.StringBuilder
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ")
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1)
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3)
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by $r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>()
virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10) is dominated by virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10)
return is dominated by r0 := @parameter0: java.lang.String[]
return is dominated by $i2 = lengthof r0
return is dominated by if $i2 >= 2 goto $r1 = r0[0]
return is dominated by $r1 = r0[0]
return is dominated by i0 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r1)
return is dominated by $r2 = r0[1]
return is dominated by i1 = staticinvoke <java.lang.Integer: int parseInt(java.lang.String)>($r2)
return is dominated by $r4 = <java.lang.System: java.io.PrintStream out>
return is dominated by $r3 = new java.lang.StringBuilder
return is dominated by specialinvoke $r3.<java.lang.StringBuilder: void <init>(java.lang.String)>("gcd(")
return is dominated by $r5 = virtualinvoke $r3.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i0)
return is dominated by $r6 = virtualinvoke $r5.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(", ")
return is dominated by $r7 = virtualinvoke $r6.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>(i1)
return is dominated by $r8 = virtualinvoke $r7.<java.lang.StringBuilder: java.lang.StringBuilder append(java.lang.String)>(") = ")
return is dominated by $i3 = staticinvoke <a1.GCD: int gcd(int,int)>(i0, i1)
return is dominated by $r9 = virtualinvoke $r8.<java.lang.StringBuilder: java.lang.StringBuilder append(int)>($i3)
return is dominated by $r10 = virtualinvoke $r9.<java.lang.StringBuilder: java.lang.String toString()>()
return is dominated by virtualinvoke $r4.<java.io.PrintStream: void println(java.lang.String)>($r10)
return is dominated by return
i0 := @parameter0: int is dominated by i0 := @parameter0: int
i1 := @parameter1: int is dominated by i0 := @parameter0: int
i1 := @parameter1: int is dominated by i1 := @parameter1: int
if i0 <= i1 goto i8 = i0 is dominated by i0 := @parameter0: int
if i0 <= i1 goto i8 = i0 is dominated by i1 := @parameter1: int
if i0 <= i1 goto i8 = i0 is dominated by if i0 <= i1 goto i8 = i0
i7 = i1 is dominated by i0 := @parameter0: int
i7 = i1 is dominated by i1 := @parameter1: int
i7 = i1 is dominated by if i0 <= i1 goto i8 = i0
i7 = i1 is dominated by i7 = i1
goto [?= (branch)] is dominated by i0 := @parameter0: int
goto [?= (branch)] is dominated by i1 := @parameter1: int
goto [?= (branch)] is dominated by if i0 <= i1 goto i8 = i0
goto [?= (branch)] is dominated by i7 = i1
goto [?= (branch)] is dominated by goto [?= (branch)]
$i5 = i0 % i7 is dominated by i0 := @parameter0: int
$i5 = i0 % i7 is dominated by i1 := @parameter1: int
$i5 = i0 % i7 is dominated by if i0 <= i1 goto i8 = i0
$i5 = i0 % i7 is dominated by i7 = i1
$i5 = i0 % i7 is dominated by goto [?= (branch)]
$i5 = i0 % i7 is dominated by $i5 = i0 % i7
$i5 = i0 % i7 is dominated by if i7 >= 1 goto $i5 = i0 % i7
if $i5 != 0 goto i7 = i7 + -1 is dominated by i0 := @parameter0: int
if $i5 != 0 goto i7 = i7 + -1 is dominated by i1 := @parameter1: int
if $i5 != 0 goto i7 = i7 + -1 is dominated by if i0 <= i1 goto i8 = i0
if $i5 != 0 goto i7 = i7 + -1 is dominated by i7 = i1
if $i5 != 0 goto i7 = i7 + -1 is dominated by goto [?= (branch)]
if $i5 != 0 goto i7 = i7 + -1 is dominated by $i5 = i0 % i7
if $i5 != 0 goto i7 = i7 + -1 is dominated by if $i5 != 0 goto i7 = i7 + -1
if $i5 != 0 goto i7 = i7 + -1 is dominated by if i7 >= 1 goto $i5 = i0 % i7
$i6 = i1 % i7 is dominated by i0 := @parameter0: int
$i6 = i1 % i7 is dominated by i1 := @parameter1: int
$i6 = i1 % i7 is dominated by if i0 <= i1 goto i8 = i0
$i6 = i1 % i7 is dominated by i7 = i1
$i6 = i1 % i7 is dominated by goto [?= (branch)]
$i6 = i1 % i7 is dominated by $i5 = i0 % i7
$i6 = i1 % i7 is dominated by if $i5 != 0 goto i7 = i7 + -1
$i6 = i1 % i7 is dominated by $i6 = i1 % i7
$i6 = i1 % i7 is dominated by if i7 >= 1 goto $i5 = i0 % i7
if $i6 != 0 goto i7 = i7 + -1 is dominated by i0 := @parameter0: int
if $i6 != 0 goto i7 = i7 + -1 is dominated by i1 := @parameter1: int
if $i6 != 0 goto i7 = i7 + -1 is dominated by if i0 <= i1 goto i8 = i0
if $i6 != 0 goto i7 = i7 + -1 is dominated by i7 = i1
if $i6 != 0 goto i7 = i7 + -1 is dominated by goto [?= (branch)]
if $i6 != 0 goto i7 = i7 + -1 is dominated by $i5 = i0 % i7
if $i6 != 0 goto i7 = i7 + -1 is dominated by if $i5 != 0 goto i7 = i7 + -1
if $i6 != 0 goto i7 = i7 + -1 is dominated by $i6 = i1 % i7
if $i6 != 0 goto i7 = i7 + -1 is dominated by if $i6 != 0 goto i7 = i7 + -1
if $i6 != 0 goto i7 = i7 + -1 is dominated by if i7 >= 1 goto $i5 = i0 % i7
return i7 is dominated by i0 := @parameter0: int
return i7 is dominated by i1 := @parameter1: int
return i7 is dominated by if i0 <= i1 goto i8 = i0
return i7 is dominated by i7 = i1
return i7 is dominated by goto [?= (branch)]
return i7 is dominated by $i5 = i0 % i7
return i7 is dominated by if $i5 != 0 goto i7 = i7 + -1
return i7 is dominated by $i6 = i1 % i7
return i7 is dominated by if $i6 != 0 goto i7 = i7 + -1
return i7 is dominated by return i7
return i7 is dominated by if i7 >= 1 goto $i5 = i0 % i7
i7 = i7 + -1 is dominated by i0 := @parameter0: int
i7 = i7 + -1 is dominated by i1 := @parameter1: int
i7 = i7 + -1 is dominated by if i0 <= i1 goto i8 = i0
i7 = i7 + -1 is dominated by i7 = i1
i7 = i7 + -1 is dominated by goto [?= (branch)]
i7 = i7 + -1 is dominated by $i5 = i0 % i7
i7 = i7 + -1 is dominated by if $i5 != 0 goto i7 = i7 + -1
i7 = i7 + -1 is dominated by i7 = i7 + -1
i7 = i7 + -1 is dominated by if i7 >= 1 goto $i5 = i0 % i7
if i7 >= 1 goto $i5 = i0 % i7 is dominated by i0 := @parameter0: int
if i7 >= 1 goto $i5 = i0 % i7 is dominated by i1 := @parameter1: int
if i7 >= 1 goto $i5 = i0 % i7 is dominated by if i0 <= i1 goto i8 = i0
if i7 >= 1 goto $i5 = i0 % i7 is dominated by i7 = i1
if i7 >= 1 goto $i5 = i0 % i7 is dominated by goto [?= (branch)]
if i7 >= 1 goto $i5 = i0 % i7 is dominated by if i7 >= 1 goto $i5 = i0 % i7
goto [?= return 1] is dominated by i0 := @parameter0: int
goto [?= return 1] is dominated by i1 := @parameter1: int
goto [?= return 1] is dominated by if i0 <= i1 goto i8 = i0
goto [?= return 1] is dominated by i7 = i1
goto [?= return 1] is dominated by goto [?= (branch)]
goto [?= return 1] is dominated by if i7 >= 1 goto $i5 = i0 % i7
goto [?= return 1] is dominated by goto [?= return 1]
i8 = i0 is dominated by i0 := @parameter0: int
i8 = i0 is dominated by i1 := @parameter1: int
i8 = i0 is dominated by if i0 <= i1 goto i8 = i0
i8 = i0 is dominated by i8 = i0
goto [?= (branch)] is dominated by i0 := @parameter0: int
goto [?= (branch)] is dominated by i1 := @parameter1: int
goto [?= (branch)] is dominated by if i0 <= i1 goto i8 = i0
goto [?= (branch)] is dominated by i8 = i0
goto [?= (branch)] is dominated by goto [?= (branch)]
$i3 = i0 % i8 is dominated by i0 := @parameter0: int
$i3 = i0 % i8 is dominated by i1 := @parameter1: int
$i3 = i0 % i8 is dominated by if i0 <= i1 goto i8 = i0
$i3 = i0 % i8 is dominated by i8 = i0
$i3 = i0 % i8 is dominated by goto [?= (branch)]
$i3 = i0 % i8 is dominated by $i3 = i0 % i8
$i3 = i0 % i8 is dominated by if i8 >= 1 goto $i3 = i0 % i8
if $i3 != 0 goto i8 = i8 + -1 is dominated by i0 := @parameter0: int
if $i3 != 0 goto i8 = i8 + -1 is dominated by i1 := @parameter1: int
if $i3 != 0 goto i8 = i8 + -1 is dominated by if i0 <= i1 goto i8 = i0
if $i3 != 0 goto i8 = i8 + -1 is dominated by i8 = i0
if $i3 != 0 goto i8 = i8 + -1 is dominated by goto [?= (branch)]
if $i3 != 0 goto i8 = i8 + -1 is dominated by $i3 = i0 % i8
if $i3 != 0 goto i8 = i8 + -1 is dominated by if $i3 != 0 goto i8 = i8 + -1
if $i3 != 0 goto i8 = i8 + -1 is dominated by if i8 >= 1 goto $i3 = i0 % i8
$i4 = i1 % i8 is dominated by i0 := @parameter0: int
$i4 = i1 % i8 is dominated by i1 := @parameter1: int
$i4 = i1 % i8 is dominated by if i0 <= i1 goto i8 = i0
$i4 = i1 % i8 is dominated by i8 = i0
$i4 = i1 % i8 is dominated by goto [?= (branch)]
$i4 = i1 % i8 is dominated by $i3 = i0 % i8
$i4 = i1 % i8 is dominated by if $i3 != 0 goto i8 = i8 + -1
$i4 = i1 % i8 is dominated by $i4 = i1 % i8
$i4 = i1 % i8 is dominated by if i8 >= 1 goto $i3 = i0 % i8
if $i4 != 0 goto i8 = i8 + -1 is dominated by i0 := @parameter0: int
if $i4 != 0 goto i8 = i8 + -1 is dominated by i1 := @parameter1: int
if $i4 != 0 goto i8 = i8 + -1 is dominated by if i0 <= i1 goto i8 = i0
if $i4 != 0 goto i8 = i8 + -1 is dominated by i8 = i0
if $i4 != 0 goto i8 = i8 + -1 is dominated by goto [?= (branch)]
if $i4 != 0 goto i8 = i8 + -1 is dominated by $i3 = i0 % i8
if $i4 != 0 goto i8 = i8 + -1 is dominated by if $i3 != 0 goto i8 = i8 + -1
if $i4 != 0 goto i8 = i8 + -1 is dominated by $i4 = i1 % i8
if $i4 != 0 goto i8 = i8 + -1 is dominated by if $i4 != 0 goto i8 = i8 + -1
if $i4 != 0 goto i8 = i8 + -1 is dominated by if i8 >= 1 goto $i3 = i0 % i8
return i8 is dominated by i0 := @parameter0: int
return i8 is dominated by i1 := @parameter1: int
return i8 is dominated by if i0 <= i1 goto i8 = i0
return i8 is dominated by i8 = i0
return i8 is dominated by goto [?= (branch)]
return i8 is dominated by $i3 = i0 % i8
return i8 is dominated by if $i3 != 0 goto i8 = i8 + -1
return i8 is dominated by $i4 = i1 % i8
return i8 is dominated by if $i4 != 0 goto i8 = i8 + -1
return i8 is dominated by return i8
return i8 is dominated by if i8 >= 1 goto $i3 = i0 % i8
i8 = i8 + -1 is dominated by i0 := @parameter0: int
i8 = i8 + -1 is dominated by i1 := @parameter1: int
i8 = i8 + -1 is dominated by if i0 <= i1 goto i8 = i0
i8 = i8 + -1 is dominated by i8 = i0
i8 = i8 + -1 is dominated by goto [?= (branch)]
i8 = i8 + -1 is dominated by $i3 = i0 % i8
i8 = i8 + -1 is dominated by if $i3 != 0 goto i8 = i8 + -1
i8 = i8 + -1 is dominated by i8 = i8 + -1
i8 = i8 + -1 is dominated by if i8 >= 1 goto $i3 = i0 % i8
if i8 >= 1 goto $i3 = i0 % i8 is dominated by i0 := @parameter0: int
if i8 >= 1 goto $i3 = i0 % i8 is dominated by i1 := @parameter1: int
if i8 >= 1 goto $i3 = i0 % i8 is dominated by if i0 <= i1 goto i8 = i0
if i8 >= 1 goto $i3 = i0 % i8 is dominated by i8 = i0
if i8 >= 1 goto $i3 = i0 % i8 is dominated by goto [?= (branch)]
if i8 >= 1 goto $i3 = i0 % i8 is dominated by if i8 >= 1 goto $i3 = i0 % i8
return 1 is dominated by i0 := @parameter0: int
return 1 is dominated by i1 := @parameter1: int
return 1 is dominated by if i0 <= i1 goto i8 = i0
return 1 is dominated by return 1

### Part 2

CHA:

<a1.Example: a1.Animal selectAnimal()> may call <a1.Cat: void <init>()>
<a1.Example: void main(java.lang.String[])> may call <a1.Example: a1.Animal selectAnimal()>
Total Edges:12<a1.Example: void main(java.lang.String[])> may call <a1.Cat: void saySomething()>
<a1.Example: void main(java.lang.String[])> may call <a1.Fish: void saySomething()>
<a1.Animal: void <init>()> may call <java.lang.Object: void <init>()>
<a1.Fish: void saySomething()> may call <java.lang.System: void <clinit>()>
<a1.Fish: void saySomething()> may call <java.io.PrintStream: void println(java.lang.String)>
<a1.Fish: void saySomething()> may call <java.lang.Object: void <clinit>()>
<a1.Cat: void <init>()> may call <a1.Animal: void <init>()>
<a1.Cat: void saySomething()> may call <java.lang.System: void <clinit>()>
<a1.Cat: void saySomething()> may call <java.io.PrintStream: void println(java.lang.String)>
<a1.Cat: void saySomething()> may call <java.lang.Object: void <clinit>()>

PTA:
<a1.Example: a1.Animal selectAnimal()> may call <a1.Cat: void <init>()>
<a1.Example: void main(java.lang.String[])> may call <a1.Example: a1.Animal selectAnimal()>
<a1.Example: void main(java.lang.String[])> may call <a1.Cat: void saySomething()>
Total Edges:7
<a1.Animal: void <init>()> may call <java.lang.Object: void <init>()>
<a1.Cat: void <init>()> may call <a1.Animal: void <init>()>
<a1.Cat: void saySomething()> may call <java.lang.System: void <clinit>()>
<a1.Cat: void saySomething()> may call <java.lang.Object: void <clinit>()>

On my computer, both class hierarchy analysis and points-to analysis finish running in about the same amount of time, 5-7 seconds.
Class hierarchy analysis is definitely less precise, showing that the example program could be calling either Cat.saySomething() or Fish.saySomething().
Points-to analysis is more precise, showing that Cat.saySomething() is the only method being called.


#### Part 3

r1 = staticinvoke <a1.Example: a1.Animal selectAnimal()>()
virtualinvoke r1.<a1.Animal: void saySomething()>()

