# Ini File Handler for Cerberus X

This is a simple ini file handler which currently supports reading only for all platforms.

Example usage:

    Local ini:IniHandler = New IniHandler()
    ini.Open("config.ini")
    
    Local str:String = ini.ReadValue("General", "TestString", "default")
    Local f:Float = ini.ReadValue("General", "TestFloat", 1.0)
    Local i:Int = ini.ReadValue("General", "TestInt", 1) + "'"
    Local b:Bool = ini.ReadValue("General", "TestBool", False)
    Local iarr:Int[]   = ini.ReadArray("General", "IntArr", [1, 2, 3])
    Local farr:Float[] = ini.ReadArray("General", "FloatArr", [1.0, 2.0, 3.0])
    Local barr:Bool[]  = ini.ReadArray("General", "BoolArr", [True, False, True])
