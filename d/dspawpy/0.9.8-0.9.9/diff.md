# Comparing `tmp/dspawpy-0.9.8-py3-none-any.whl.zip` & `tmp/dspawpy-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,20 @@
-Zip file size: 75131 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-09 09:28 dspawpy/__init__.py
--rw-rw-rw-  2.0 fat    30667 b- defN 23-Jun-09 09:28 dspawpy/plot.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    24367 b- defN 23-Jun-09 09:28 dspawpy/analysis/aimdtools.py
--rw-rw-rw-  2.0 fat    20152 b- defN 23-May-23 06:07 dspawpy/analysis/vacf.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 06:07 dspawpy/diffusion/__init__.py
--rw-rw-rw-  2.0 fat     4028 b- defN 23-Jun-09 09:28 dspawpy/diffusion/neb.py
--rw-rw-rw-  2.0 fat    56939 b- defN 23-Jun-09 09:28 dspawpy/diffusion/nebtools.py
--rw-rw-rw-  2.0 fat    11045 b- defN 23-May-23 06:07 dspawpy/diffusion/pathfinder.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
--rw-rw-rw-  2.0 fat    54091 b- defN 23-Jun-09 09:28 dspawpy/io/read.py
--rw-rw-rw-  2.0 fat     7721 b- defN 23-May-23 06:07 dspawpy/io/read_json.py
--rw-rw-rw-  2.0 fat    10317 b- defN 23-Jun-09 08:47 dspawpy/io/structure.py
--rw-rw-rw-  2.0 fat    27299 b- defN 23-Jun-09 09:28 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    29663 b- defN 23-Jun-09 09:28 dspawpy/io/write.py
--rw-rw-rw-  2.0 fat     1761 b- defN 23-May-23 06:07 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-09 09:29 dspawpy-0.9.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 09:29 dspawpy-0.9.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-09 09:29 dspawpy-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1583 b- defN 23-Jun-09 09:29 dspawpy-0.9.8.dist-info/RECORD
-20 files, 284038 bytes uncompressed, 72581 bytes compressed:  74.4%
+Zip file size: 73130 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx       22 b- defN 23-Jun-16 02:04 dspawpy/__init__.py
+-rw-rw-r--  2.0 unx    31198 b- defN 23-Jun-13 12:38 dspawpy/plot.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 05:34 dspawpy/analysis/__init__.py
+-rw-rw-r--  2.0 unx    23655 b- defN 23-Jun-13 09:06 dspawpy/analysis/aimdtools.py
+-rw-rw-r--  2.0 unx    19597 b- defN 23-Jun-13 05:34 dspawpy/analysis/vacf.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 05:34 dspawpy/diffusion/__init__.py
+-rw-rw-r--  2.0 unx     3913 b- defN 23-Jun-13 05:34 dspawpy/diffusion/neb.py
+-rw-rw-r--  2.0 unx    55591 b- defN 23-Jun-13 12:26 dspawpy/diffusion/nebtools.py
+-rw-rw-r--  2.0 unx    10758 b- defN 23-Jun-13 05:34 dspawpy/diffusion/pathfinder.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 05:34 dspawpy/io/__init__.py
+-rw-rw-r--  2.0 unx    61048 b- defN 23-Jun-16 01:41 dspawpy/io/read.py
+-rw-rw-r--  2.0 unx    10224 b- defN 23-Jun-13 12:38 dspawpy/io/structure.py
+-rw-rw-r--  2.0 unx    26350 b- defN 23-Jun-13 05:34 dspawpy/io/utils.py
+-rw-rw-r--  2.0 unx    28766 b- defN 23-Jun-13 05:34 dspawpy/io/write.py
+-rw-rw-r--  2.0 unx     4513 b- defN 23-Jun-16 02:04 dspawpy-0.9.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 02:04 dspawpy-0.9.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-16 02:04 dspawpy-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1422 b- defN 23-Jun-16 02:04 dspawpy-0.9.9.dist-info/RECORD
+18 files, 277157 bytes uncompressed, 70826 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -27,35 +27,29 @@
 
 Filename: dspawpy/io/__init__.py
 Comment: 
 
 Filename: dspawpy/io/read.py
 Comment: 
 
-Filename: dspawpy/io/read_json.py
-Comment: 
-
 Filename: dspawpy/io/structure.py
 Comment: 
 
 Filename: dspawpy/io/utils.py
 Comment: 
 
 Filename: dspawpy/io/write.py
 Comment: 
 
-Filename: dspawpy/io/write_json.py
-Comment: 
-
-Filename: dspawpy-0.9.8.dist-info/METADATA
+Filename: dspawpy-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.9.8.dist-info/WHEEL
+Filename: dspawpy-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.9.8.dist-info/top_level.txt
+Filename: dspawpy-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.9.8.dist-info/RECORD
+Filename: dspawpy-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.9.8"
+__version__ = "0.9.9"
```

## dspawpy/plot.py

```diff
@@ -1,824 +1,862 @@
-import json
-import os
-
-import h5py
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-from scipy.interpolate import interp1d
-
-from dspawpy.io.read import load_h5
-
-
-def average_along_axis(
-    datafile="potential.h5",
-    task: str = "potential",
-    axis=2,
-    smooth=False,
-    smooth_frac=0.8,
-    raw=False,
-    **kwargs,
-):
-    r"""绘制沿着某个轴向的物理量平均值曲线
-
-    Parameters
-    ----------
-    datafile : str or list or np.ndarray
-        h5或json文件路径或包含任意这些文件的文件夹，默认 'potential.h5'
-    task: str
-        任务类型，可以是 'rho', 'potential', 'elf', 'pcharge', 'boundcharge'
-    axis : int
-        沿着哪个轴向绘制势能曲线, 默认2
-    smooth : bool
-        是否平滑, 默认False
-    smooth_frac : float
-        平滑系数, 默认0.8
-    raw : bool
-        是否返回原始数据到csv文件
-    **kwargs : dict
-        其他参数, 传递给 matplotlib.pyplot.plot
-
-    Returns
-    -------
-    axes: matplotlib.axes._subplots.AxesSubplot
-        可传递给其他函数进行进一步处理
-
-    Examples
-    --------
-    >>> from dspawpy.plot import average_along_axis
-
-    读取 potential.h5 文件中的数据，绘图并保存原始绘图数据到csv文件
-
-    >>> average_along_axis(datafile='/data/home/hzw1002/dspawpy_repo/test/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8, raw=True)
-    <module 'matplotlib.pyplot' from '/data/home/hzw1002/anaconda3/lib/python3.9/site-packages/matplotlib/pyplot.py'>
-    """
-    assert task.lower() in [
-        "rho",
-        "potential",
-        "elf",
-        "pcharge",
-        "boundcharge",
-    ], "仅支持 rho, potential, elf, pcharge, boundcharge 任务类型"
-    # only for compatibility
-    if isinstance(datafile, list) or isinstance(datafile, np.ndarray):
-        ys = datafile  # expect np.ndarray or list
-
-    # search datafile in the given directory
-    elif os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, f"{task}.h5")):
-            datafile = os.path.join(directory, f"{task}.h5")
-            print("Readingf {task}.h5...")
-        elif os.path.exists(os.path.join(directory, f"{task}.json")):
-            datafile = os.path.join(directory, f"{task}.json")
-            print("Readingf {task}.json...")
-        else:
-            raise FileNotFoundError(f"未找到{task}.h5/{task}.json文件！")
-
-    # parse the real datafile
-    elif datafile.endswith(".h5"):
-        hfile = datafile
-        hdict = load_h5(hfile)
-        grid = hdict["/AtomInfo/Grid"]
-        # pot = np.asarray(potential["/Potential/TotalElectrostaticPotential"]).reshape(grid, order="F")
-        # DS-PAW 数据写入h5 列优先
-        # h5py 从h5读取数据 默认行优先
-        # np.array(data_list) 默认行优先
-        # 所以这里先以 行优先 把 “h5 行优先 读进来的数据” 转成一维， 再以 列优先 转成 grid 对应的维度
-        if task.lower() == "rho":
-            key = "/Rho/TotalCharge"
-        elif task.lower() == "potential":
-            key = "/Potential/TotalElectrostaticPotential"
-        elif task.lower() == "elf":
-            key = "/ELF/TotalELF"
-        elif task.lower() == "pcharge":
-            key = "/Pcharge/1/TotalCharge"
-        else:
-            key = "/Rho"
-        tmp_pot = np.asarray(hdict[key]).reshape([-1, 1], order="C")
-        ys = tmp_pot.reshape(grid, order="F")
-
-    elif datafile.endswith(".json"):
-        jfile = datafile
-        with open(jfile, "r") as f:
-            jdict = json.load(f)
-        grid = jdict["AtomInfo"]["Grid"]
-
-        if task.lower() == "rho":
-            ys = np.asarray(jdict["Rho"]["TotalCharge"]).reshape(grid, order="F")
-        elif task.lower() == "potential":
-            ys = np.asarray(jdict["Potential"]["TotalElectrostaticPotential"]).reshape(
-                grid, order="F"
-            )
-        elif task.lower() == "elf":
-            ys = np.asarray(jdict["ELF"]["TotalELF"]).reshape(grid, order="F")
-        elif task.lower() == "pcharge":
-            ys = np.asarray(jdict["Pcharge"][0]["TotalCharge"]).reshape(grid, order="F")
-        else:
-            ys = np.asarray(jdict["Rho"]).reshape(grid, order="F")
-
-    else:
-        raise TypeError("仅支持读取h5或json文件或直接传入数组！")
-
-    all_axis = [0, 1, 2]
-    all_axis.remove(axis)
-    y = np.mean(ys, tuple(all_axis))
-    x = np.arange(len(y))
-
-    if raw:
-        pd.DataFrame({"x": x, "y": y}).to_csv(f"raw{task}_axis{axis}.csv", index=False)
-    if smooth:
-        s = sm.nonparametric.lowess(y, x, frac=smooth_frac)
-        if raw:
-            pd.DataFrame({"x": s[:, 0], "y": s[:, 1]}).to_csv(
-                f"raw{task}_axis{axis}_smooth.csv", index=False
-            )
-
-        plt.plot(s[:, 0], s[:, 1], label="macroscopic average", **kwargs)
-
-    plt.plot(x, y, **kwargs)
-
-    return plt
-
-
-def plot_aimd(
-    datafile: str = "aimd.h5",
-    show: bool = True,
-    figname: str = "aimd.png",
-    flags_str="12345",
-    raw=False,
-):
-    r"""AIMD任务完成后，绘制关键物理量的收敛过程图
-
-    aimd.h5 -> aimd.png
-
-    Parameters
-    ----------
-    datafile : str or list
-        h5文件位置. 例如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
-    show : bool
-        是否展示交互界面. 默认 False
-    figname : str
-        保存的图片路径. 默认 'aimd.h5'
-    flags_str : str
-        子图编号.
-        1. 动能
-        2. 总能
-        3. 压力
-        4. 温度
-        5. 体积
-    raw : bool
-        是否输出原始数据到csv文件
-
-    Returns
-    ----------
-    figname : str
-        图片路径，默认 'aimd.png'
-
-    Examples
-    ----------
-    >>> from dspawpy.plot import plot_aimd
-
-    读取 aimd.h5 文件内容，画出动能、总能、温度、体积的收敛过程图，并保存相应数据到 rawaimd_*.csv 中
-
-    >>> plot_aimd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', flags_str='1245', raw=False, show=False, figname=None)
-    正在处理子图1
-     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    正在处理子图2
-     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    正在处理子图4
-     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    正在处理子图5
-     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    """
-    # 处理用户读取，按顺序去重
-    temp = set()
-    flags = [x for x in flags_str if x not in temp and (temp.add(x) or True)]
-    if " " in flags:  # remove space
-        flags.remove(" ")
-
-    for flag in flags:
-        assert flag in ["1", "2", "3", "4", "5"], "读取错误！"
-
-    # 开始画组合图
-    N_figs = len(flags)
-    fig, axes = plt.subplots(N_figs, 1, sharex=True, figsize=(6, 2 * N_figs))
-    if N_figs == 1:  # 'AxesSubplot' object is not subscriptable
-        axes = [axes]  # 避免上述类型错误
-    fig.suptitle("DSPAW AIMD")
-    for i, flag in enumerate(flags):
-        print("正在处理子图" + flag)
-        # 读取数据
-        xs, ys = _read_aimd_converge_data(datafile, flag)
-        if raw:
-            pd.DataFrame({"x": xs, "y": ys}).to_csv(f"rawaimd_{flag}.csv", index=False)
-
-        axes[i].plot(xs, ys)  # 绘制坐标点
-        # 子图的y轴标签
-        if flag == "1":
-            axes[i].set_ylabel("Kinetic Energy (eV)")
-        elif flag == "2":
-            axes[i].set_ylabel("Energy (eV)")
-        elif flag == "3":
-            axes[i].set_ylabel("Pressure Kinetic (kbar)")
-        elif flag == "4":
-            axes[i].set_ylabel("Temperature (K)")
-        else:
-            axes[i].set_ylabel("Volume (Angstrom^3)")
-
-    plt.tight_layout()
-    # save and show
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
-    if show:
-        plt.show()
-
-
-def plot_bandunfolding(
-    datafile: str = "band.h5", ef=0.0, de=0.05, dele=0.06, raw=False
-):
-    r"""能带反折叠任务完成后，读取 h5 或 json 文件数据绘图
-
-    band.h5/band.json -> bandunfolding.png
-
-    Parameters
-    ----------
-    datafile : str
-        h5或json文件路径或包含任意这些文件的文件夹，默认 'band.h5'
-    ef : float
-        费米能级，默认置于 y = 0 处
-    de : float
-        能带宽度，默认0.05
-    dele : float
-        能带间隔，默认0.06
-    raw : bool
-        是否输出原始数据到rawbandunfolding.csv
-
-    Returns
-    -------
-    axes: matplotlib.axes._subplots.AxesSubplot
-        可传递给其他函数进行进一步处理
-
-    Examples
-    --------
-
-    绘图并保存原始数据到rawbandunfolding.csv
-
-    >>> from dspawpy.plot import plot_bandunfolding
-    >>> plot_bandunfolding("/data/home/hzw1002/dspawpy_repo/test/2.22/band.h5", raw=True)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.22/band.h5...
-    <module 'matplotlib.pyplot' from '/data/home/hzw1002/anaconda3/lib/python3.9/site-packages/matplotlib/pyplot.py'>
-    """
-    # search datafile in the given directory
-    if os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, "band.h5")):
-            datafile = os.path.join(directory, "band.h5")
-            print("Reading band.h5...")
-        elif os.path.exists(os.path.join(directory, "band.json")):
-            datafile = os.path.join(directory, "band.json")
-            print("Reading band.json...")
-        else:
-            raise FileNotFoundError("未找到band.h5/band.json文件！")
-
-    if datafile.endswith(".h5"):
-        # band = load_h5(datafile)
-        import h5py
-
-        print(f"Reading {os.path.abspath(datafile)}...")
-        f = h5py.File(datafile, "r")
-        number_of_band = np.array(f["/BandInfo/NumberOfBand"])[0]
-        # number_of_band = band["/BandInfo/NumberOfBand"][0]
-        number_of_kpoints = np.array(f["/BandInfo/NumberOfKpoints"])[0]
-        # number_of_kpoints = band["/BandInfo/NumberOfKpoints"][0]
-        data = np.array(f["/UnfoldingBandInfo/Spin1/UnfoldingBand"])
-        # data = band["/UnfoldingBandInfo/Spin1/UnfoldingBand"]
-        weight = np.array(f["/UnfoldingBandInfo/Spin1/Weight"])
-        # weight = band["/UnfoldingBandInfo/Spin1/Weight"]
-    elif datafile.endswith(".json"):
-        with open(datafile, "r") as f:
-            band = json.load(f)
-        number_of_band = band["BandInfo"]["NumberOfBand"]
-        number_of_kpoints = band["BandInfo"]["NumberOfKpoints"]
-        data = band["UnfoldingBandInfo"]["Spin1"]["UnfoldingBand"]
-        weight = band["UnfoldingBandInfo"]["Spin1"]["Weight"]
-    else:
-        raise TypeError("仅支持读取h5或json文件！")
-
-    celtot = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-    proj_wt = np.array(weight).reshape((number_of_kpoints, number_of_band)).T
-    X2, Y2, Z2, emin = getEwtData(
-        number_of_kpoints, number_of_band, celtot, proj_wt, ef, de, dele
-    )
-
-    if raw:
-        pd.DataFrame({"Y": Y2, "Z": Z2}, index=X2).to_csv(
-            "rawbandunfolding.csv", header=["Y", "color"], index=True, index_label="X"
-        )
-
-    plt.scatter(X2, Y2, c=Z2, cmap="hot")
-    plt.xlim(0, 200)
-    plt.ylim(emin - 0.5, 15)
-    ax = plt.gca()
-    plt.colorbar()
-    ax.set_facecolor("black")
-
-    return plt
-
-
-def plot_optical(
-    datafile: str = "optical.h5",
-    key: str = "AbsorptionCoefficient",
-    index: int = 0,
-    raw=False,
-):
-    """光学性质计算任务完成后，读取数据并绘制预览图
-
-    optical.h5/optical.json -> optical.png
-
-    Parameters
-    ----------
-    datafile : str
-        h5或json文件路径或包含任意这些文件的文件夹，默认 'optical.h5'
-    key: str
-        可选 "AbsorptionCoefficient", "ExtinctionCoefficient", "RefractiveIndex", "Reflectance" 中的任意一个，默认 "AbsorptionCoefficient"
-    index : int
-        序号，默认0
-    raw : bool
-        是否保存原始数据到csv
-
-    Returns
-    -------
-    axes: matplotlib.axes._subplots.AxesSubplot
-        可传递给其他函数进行进一步处理
-
-    Examples
-    --------
-
-    绘图并保存原始数据到rawoptical.csv
-
-    >>> from dspawpy.plot import plot_optical
-    >>> plot_optical("/data/home/hzw1002/dspawpy_repo/test/2.12/scf.h5", "AbsorptionCoefficient", 0, raw=True)
-    >>> plot_optical("/data/home/hzw1002/dspawpy_repo/test/2.12/optical.json", "AbsorptionCoefficient", 0, raw=True)
-    """
-    # search datafile in the given directory
-    if os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, "optical.h5")):
-            datafile = os.path.join(directory, "optical.h5")
-            print("Reading optical.h5...")
-        elif os.path.exists(os.path.join(directory, "optical.json")):
-            datafile = os.path.join(directory, "optical.json")
-            print("Reading optical.json...")
-        else:
-            raise FileNotFoundError("未找到optical.h5/optical.json文件！")
-
-    # parse the real datafile
-    if datafile.endswith("h5"):
-        data_all = load_h5(datafile)
-        energy = data_all["/OpticalInfo/EnergyAxe"]
-        data = data_all["/OpticalInfo/" + key]
-    elif datafile.endswith("json"):
-        with open(datafile, "r") as fin:
-            data_all = json.load(fin)
-        energy = data_all["OpticalInfo"]["EnergyAxe"]
-        data = data_all["OpticalInfo"][key]
-    else:
-        raise TypeError("仅支持读取h5或json文件！")
-
-    data = np.asarray(data).reshape(len(energy), 6)[:, index]
-    inter_f = interp1d(energy, data, kind="cubic")
-    energy_spline = np.linspace(energy[0], energy[-1], 2001)
-    data_spline = inter_f(energy_spline)
-
-    if raw:
-        pd.DataFrame({"energy": energy, "data": data}).to_csv(
-            "rawoptical.csv", index=False
-        )
-        pd.DataFrame(
-            {"energy_spline": energy_spline, "data_spline": data_spline}
-        ).to_csv("rawoptical_spline.csv", index=False)
-
-    plt.plot(energy_spline, data_spline, c="b")
-    plt.xlabel("Photon energy (eV)")
-    plt.ylabel("%s %s" % (key, r"$\alpha (\omega )(cm^{-1})$"))
-
-
-def plot_phonon_thermal(
-    datafile: str = "phonon.h5",
-    figname: str = "phonon.png",
-    show: bool = True,
-    raw=False,
-):
-    """声子热力学计算任务完成后，绘制相关物理量随温度变化曲线
-
-    phonon.h5/phonon.json -> phonon.png
-
-    Parameters
-    ----------
-    datafile : str
-        h5或json文件路径或包含任意这些文件的文件夹，默认 'phonon.h5'
-    figname : str
-        保存图片的文件名
-    show : bool
-        是否弹出交互界面
-    raw : bool
-        是否保存原始数据到rawphonon.csv文件
-
-    Returns
-    ----------
-    figname : str
-        图片路径，默认 'phonon.png'
-
-    Examples
-    --------
-    >>> from dspawpy.plot import plot_phonon_thermal
-    >>> plot_phonon_thermal('/data/home/hzw1002/dspawpy_repo/test/2.26/phonon.h5', figname='/data/home/hzw1002/dspawpy_repo/test/out/phonon_thermal.png', show=False)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.26/phonon.h5...
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/out/phonon_thermal.png
-    """
-    # search datafile in the given directory
-    if os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, "phonon.h5")):
-            datafile = os.path.join(directory, "phonon.h5")
-            print("Reading phonon.h5...")
-        elif os.path.exists(os.path.join(directory, "phonon.json")):
-            datafile = os.path.join(directory, "phonon.json")
-            print("Reading phonon.json...")
-        else:
-            raise FileNotFoundError("未找到phonon.h5/phonon.json文件！")
-
-    if datafile.endswith(".h5"):
-        hfile = datafile
-        ph = h5py.File(hfile, "r")
-        print(f"Reading {hfile}...")
-        if "/ThermalInfo/Temperatures" not in ph:
-            raise KeyError(
-                "❓ No thermal info in datafile, you probably gave a wrong phonon.h5 file"
-            )
-        temp = np.array(ph["/ThermalInfo/Temperatures"])
-        entropy = np.array(ph["/ThermalInfo/Entropy"])
-        heat_capacity = np.array(ph["/ThermalInfo/HeatCapacity"])
-        helmholts_free_energy = np.array(ph["/ThermalInfo/HelmholtzFreeEnergy"])
-    elif datafile.endswith(".json"):
-        jfile = datafile
-        with open(jfile, "r") as f:
-            data = json.load(f)
-        print(f"Reading {jfile}...")
-        temp = np.array(data["ThermalInfo"]["Temperatures"])
-        entropy = np.array(data["ThermalInfo"]["Entropy"])
-        heat_capacity = np.array(data["ThermalInfo"]["HeatCapacity"])
-        helmholts_free_energy = np.array(data["ThermalInfo"]["HelmholtzFreeEnergy"])
-    else:
-        raise TypeError("仅支持读取h5或json文件！")
-
-    if raw:
-        pd.DataFrame(
-            {
-                "temp": temp,
-                "entropy": entropy,
-                "heat_capacity": heat_capacity,
-                "helmholts_free_energy": helmholts_free_energy,
-            }
-        ).to_csv("rawphonon.csv", index=False)
-
-    plt.plot(temp, entropy, c="red", label="Entropy (J/K/mol)")
-    plt.plot(temp, heat_capacity, c="green", label="Heat Capacity (J/K/mol)")
-    plt.plot(
-        temp, helmholts_free_energy, c="blue", label="Helmholtz Free Energy (kJ/mol)"
-    )
-    plt.xlabel("Temperature(K)")
-    plt.ylabel("Thermal Properties")
-    plt.tick_params(direction="in")  # 刻度线朝内
-    plt.grid(alpha=0.2)
-    plt.legend()
-    plt.title("Thermal")
-
-    plt.tight_layout()
-    # save and show
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
-    if show:
-        plt.show()
-
-
-def plot_polarization_figure(
-    directory: str,
-    repetition: int = 2,
-    annotation: bool = False,
-    annotation_style: int = 1,
-    show: bool = True,
-    figname: str = "pol.png",
-    raw=False,
-):
-    """绘制铁电极化结果图
-
-    Parameters
-    ----------
-    directory : str
-        铁电极化计算任务主目录
-    repetition : int
-        沿上（或下）方向重复绘制的次数, 默认 2
-    annotation : bool
-        是否显示首尾构型的铁电极化数值, 默认显示
-    show : bool
-        是否交互显示图片, 默认 True
-    figname : str
-        图片保存路径, 默认 'pol.png'
-    raw : bool
-        是否将原始数据保存到csv文件
-
-    Returns
-    -------
-    axes: matplotlib.axes._subplots.AxesSubplot
-        可传递给其他函数进行进一步处理
-
-    Examples
-    --------
-    >>> from dspawpy.plot import plot_polarization_figure
-    >>> plot_polarization_figure(directory='/data/home/hzw1002/dspawpy_repo/test/2.20', figname='/data/home/hzw1002/dspawpy_repo/test/out/pol.png', show=False)
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/out/pol.png
-    array([<Axes: title={'center': 'Px'}>, <Axes: title={'center': 'Py'}>,
-           <Axes: title={'center': 'Pz'}>], dtype=object)
-    """
-    assert repetition >= 0, "重复次数必须是自然数"
-    subfolders, quantum, totals = _get_subfolders_quantum_totals(directory)
-    number_sfs = [int(sf) for sf in subfolders]
-    fig, axes = plt.subplots(1, 3, sharey=True)
-    xyz = ["x", "y", "z"]
-    for j in range(3):  # x, y, z
-        ys = np.empty(shape=(len(subfolders), repetition * 2 + 1))
-        for r in range(repetition + 1):
-            ys[:, repetition - r] = totals[:, j] - quantum[j] * r
-            ys[:, repetition + r] = totals[:, j] + quantum[j] * r
-
-        axes[j].plot(number_sfs, ys, ".")  # plot
-        axes[j].set_title("P%s" % xyz[j])
-        axes[j].xaxis.set_ticks(number_sfs)  # 设置x轴刻度
-        axes[j].set_xticklabels(labels=subfolders, rotation=90)
-        axes[j].grid(axis="x", color="gray", linestyle=":", linewidth=0.5)
-        axes[j].tick_params(direction="in")
-        # set y ticks using the first and last values
-        if annotation:
-            if annotation_style == 2:
-                style = "arc,angleA=-0,angleB=0,armA=-10,armB=0,rad=0"
-                for i in range(repetition * 2 + 1):
-                    axes[j].annotate(
-                        f"{ys[0,i]:.2f}",
-                        xy=(number_sfs[0], ys[0, i]),
-                        xycoords="data",
-                        xytext=(number_sfs[-1] + 2, ys[0, i] - 8),
-                        textcoords="data",
-                        arrowprops=dict(
-                            arrowstyle="->",
-                            color="black",
-                            linewidth=0.75,
-                            shrinkA=2,
-                            shrinkB=1,
-                            connectionstyle=style,
-                        ),
-                    )
-                    axes[j].annotate(
-                        f"{ys[-1,i]:.2f}",
-                        xy=(number_sfs[-1], ys[-1, i]),
-                        xycoords="data",
-                        xytext=(number_sfs[-1] + 2, ys[-1, i] + 8),
-                        textcoords="data",
-                        arrowprops=dict(
-                            arrowstyle="->",
-                            color="black",
-                            linewidth=0.75,
-                            shrinkA=2,
-                            shrinkB=1,
-                            connectionstyle=style,
-                        ),
-                    )
-            elif annotation_style == 1:
-                for i in range(repetition * 2 + 1):
-                    axes[j].annotate(
-                        text=f"{ys[0,i]:.2f}",
-                        xy=(0, ys[0, i]),
-                        xytext=(0, ys[0, i] - np.max(ys) / repetition / 5),
-                    )
-                    axes[j].annotate(
-                        text=f"{ys[-1,i]:.2f}",
-                        xy=(len(subfolders) - 1, ys[-1, i]),
-                        xytext=(
-                            len(subfolders) - 1,
-                            ys[-1, i] - np.max(ys) / repetition / 5,
-                        ),
-                    )
-            else:
-                raise ValueError("annotation_style must be 1 or 2")
-
-        if raw:
-            pd.DataFrame(ys, index=subfolders).to_csv(f"pol_{xyz[j]}.csv")
-
-    plt.tight_layout()
-    # save and show
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
-    if show:
-        plt.show()
-
-    return axes
-
-
-def _get_subfolders_quantum_totals(directory: str):
-    """返回铁电极化计算任务的子目录、量子数、极化总量；
-
-    请勿创建其他子目录，否则会被错误读取
-
-    Parameters
-    ----------
-    directory：str
-        铁电极化计算任务主目录
-
-    Returns
-    -------
-    subfolders : list
-        子目录列表
-    quantum : np.ndarray
-        量子数，xyz三个方向, shape=(1, 3)
-    totals : np.ndarray
-        极化总量，xyz三个方向, shape=(len(subfolders), 3)
-    """
-
-    raw_subfolders = next(os.walk(directory))[1]
-    subfolders = []
-    for subfolder in raw_subfolders:
-        assert (
-            0 <= int(subfolder) < 100
-        ), f"--> You should rename subfolders to 0~99, but {subfolder} found"
-        try:
-            assert 0 <= int(subfolder) < 100
-            subfolders.append(subfolder)
-        except:
-            pass
-    subfolders.sort()  # 从小到大排序
-    if os.path.exists(f"{os.path.join(directory, subfolders[0])}/polarization.json"):
-        # quantum number if constant across the whole calculation,
-        # so, read only once
-        with open(
-            f"{os.path.join(directory, subfolders[0])}/polarization.json", "r"
-        ) as f:
-            quantum = json.load(f)["PolarizationInfo"]["Quantum"]
-        # the Total number is not constant
-        totals = np.empty(shape=(len(subfolders), 3))
-        for i, fd in enumerate(subfolders):
-            with open(f"{os.path.join(directory, fd)}/polarization.json", "r") as f:
-                data = json.load(f)
-            total = data["PolarizationInfo"]["Total"]
-            print("Total: ", total)
-            totals[i] = float(total)
-
-    elif os.path.exists(f"{os.path.join(directory, subfolders[0])}/scf.h5"):
-        # quantum number if constant across the whole calculation,
-        # so, read only once
-        quantum = np.array(
-            h5py.File(f"{os.path.join(directory, subfolders[0])}/scf.h5").get(
-                "/PolarizationInfo/Quantum"
-            )
-        )
-        # the Total number is not constant
-        totals = np.empty(shape=(len(subfolders), 3))
-        for i, fd in enumerate(subfolders):
-            data = h5py.File(f"{os.path.join(directory, fd)}/scf.h5")
-            total = np.array(data.get("/PolarizationInfo/Total"))
-            totals[i] = total
-    else:
-        raise ValueError("no polarization.json or scf.h5 file found")
-
-    return subfolders, quantum, totals
-
-
-def getEwtData(nk, nb, celtot, proj_wt, ef, de, dele):
-    emin = np.min(celtot) - de
-    emax = np.max(celtot) - de
-
-    emin = np.floor(emin - 0.2)
-    emax = max(np.ceil(emax) * 1.0, 5.0)
-
-    nps = int((emax - emin) / de)
-
-    X = np.zeros((nps + 1, nk))
-    Y = np.zeros((nps + 1, nk))
-
-    X2 = []
-    Y2 = []
-    Z2 = []
-
-    for ik in range(nk):
-        for ip in range(nps + 1):
-            omega = ip * de + emin + ef
-            X[ip][ik] = ik
-            Y[ip][ik] = ip * de + emin
-            ewts_value = 0
-            for ib in range(nb):
-                smearing = dele / np.pi / ((omega - celtot[ib][ik]) ** 2 + dele**2)
-                ewts_value += smearing * proj_wt[ib][ik]
-            if ewts_value > 0.01:
-                X2.append(ik)
-                Y2.append(ip * de + emin)
-                Z2.append(ewts_value)
-
-    Z2_half = max(Z2) / 2
-
-    for i, x in enumerate(Z2):
-        if x > Z2_half:
-            Z2[i] = Z2_half
-
-    return X2, Y2, Z2, emin
-
-
-def _read_aimd_converge_data(datafile: str, index: str = None):
-    """从datafile指定的路径读取index指定的数据，返回绘图用的xs和ys两个数组
-
-    Parameters
-    ----------
-    datafile : str or list
-        hdf5文件路径，如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
-    index : str
-        编号, 默认 None
-
-    Returns
-    -------
-    xs : np.ndarray
-        x轴数据
-    ys : np.ndarray
-        y轴数据
-    """
-    if isinstance(datafile, list):
-        xs = []
-        ys = []
-        for i, df in enumerate(datafile):
-            # concentrate returned np.ndarray
-            x, y = _read_aimd_converge_data(df, index)
-            xs.extend(x)
-            ys.extend(y)
-        xs = np.linspace(1, len(xs), len(xs))
-        return xs, ys
-
-    # search datafile in the given directory
-    elif isinstance(datafile, str):
-        if os.path.isdir(datafile):  # 如果是文件夹
-            directory = datafile  # specified datafile is actually a directory
-            print(f"您指定了一个文件夹，正在{directory}中自动查找aimd.h5...")
-            if os.path.exists(os.path.join(directory, "aimd.h5")):
-                datafile = os.path.join(directory, "aimd.h5")
-                print("Reading aimd.h5...")
-            else:
-                raise FileNotFoundError("未找到aimd.h5文件！")
-
-        elif datafile.endswith(".h5"):  # 如果是h5文件
-            hf = h5py.File(datafile)  # 加载h5文件
-            print(f" reading {os.path.abspath(datafile)}...")
-            Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
-            ys = np.empty(Nstep)  # 准备一个空数组
-            # 开始读取
-            if index == "5":
-                for i in range(1, Nstep + 1):
-                    ys[i - 1] = np.linalg.det(hf.get("/Structures/Step-%d/Lattice" % i))
-            else:
-                map = {
-                    "1": "IonsKineticEnergy",
-                    "2": "TotalEnergy0",
-                    "3": "PressureKinetic",
-                    "4": "Temperature",
-                }
-                for i in range(1, Nstep + 1):
-                    # 如果计算中断，则没有PressureKinetic这个键
-                    try:
-                        ys[i - 1] = np.array(
-                            hf.get("/AimdInfo/Step-%d/%s" % (i, map[index]))
-                        )
-                    except:
-                        ys[i - 1] = 0
-                        ys = np.delete(ys, -1)
-                        print(f"-> 计算中断于第 {Nstep} 步，未读取到第 {i} 步的 {map[index]} 数据！")
-                        break
-
-            Nstep = len(ys)  # 步数更新为实际完成的步数
-
-            # 返回xs，ys两个数组
-            return np.linspace(1, Nstep, Nstep), np.array(ys)
-
-        else:
-            raise TypeError("仅支持读取h5文件！")
-    else:
-        raise TypeError("datafile必须是字符串或列表！")
+import json
+import os
+
+import h5py
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+from scipy.interpolate import interp1d
+
+from dspawpy.io.read import load_h5
+
+
+def average_along_axis(
+    datafile="potential.h5",
+    task: str = "potential",
+    axis=2,
+    smooth=False,
+    smooth_frac=0.8,
+    raw=False,
+    key: str = None,
+    **kwargs,
+):
+    r"""绘制沿着某个轴向的物理量平均值曲线
+
+    Parameters
+    ----------
+    datafile : str or list or np.ndarray
+        h5或json文件路径或包含任意这些文件的文件夹，默认 'potential.h5'
+    task: str
+        任务类型，可以是 'rho', 'potential', 'elf', 'pcharge', 'boundcharge'
+    axis : int
+        沿着哪个轴向绘制势能曲线, 默认2
+    smooth : bool
+        是否平滑, 默认False
+    smooth_frac : float
+        平滑系数, 默认0.8
+    raw : bool
+        是否返回原始数据到csv文件
+    **kwargs : dict
+        其他参数, 传递给 matplotlib.pyplot.plot
+
+    Returns
+    -------
+    axes: matplotlib.axes._subplots.AxesSubplot
+        可传递给其他函数进行进一步处理
+
+    Examples
+    --------
+    >>> from dspawpy.plot import average_along_axis
+
+    读取 potential.h5 文件中的数据，绘图并保存原始绘图数据到csv文件
+
+    >>> average_along_axis(datafile='/data/home/hzw1002/dspawpy_repo/test/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8, raw=True)
+    <module 'matplotlib.pyplot' from '/data/home/hzw1002/anaconda3/lib/python3.9/site-packages/matplotlib/pyplot.py'>
+    """
+    assert task.lower() in [
+        "rho",
+        "potential",
+        "elf",
+        "pcharge",
+        "boundcharge",
+    ], "仅支持 rho, potential, elf, pcharge, boundcharge 任务类型"
+    assert key is None or isinstance(key, str), "key 必须是字符串"
+    # only for compatibility
+    if isinstance(datafile, list) or isinstance(datafile, np.ndarray):
+        ys = datafile  # expect np.ndarray or list
+
+    # search datafile in the given directory
+    elif os.path.isdir(datafile):
+        directory = datafile  # specified datafile is actually a directory
+        print("您指定了一个文件夹，正在查找相关h5或json文件...")
+        if os.path.exists(os.path.join(directory, f"{task}.h5")):
+            datafile = os.path.join(directory, f"{task}.h5")
+            print("Readingf {task}.h5...")
+        elif os.path.exists(os.path.join(directory, f"{task}.json")):
+            datafile = os.path.join(directory, f"{task}.json")
+            print("Readingf {task}.json...")
+        else:
+            raise FileNotFoundError(f"未找到{task}.h5/{task}.json文件！")
+
+    # parse the real datafile
+    elif datafile.endswith(".h5"):
+        hfile = datafile
+        hdict = load_h5(hfile)
+        grid = hdict["/AtomInfo/Grid"]
+        # pot = np.asarray(potential["/Potential/TotalElectrostaticPotential"]).reshape(grid, order="F")
+        # DS-PAW 数据写入h5 列优先
+        # h5py 从h5读取数据 默认行优先
+        # np.array(data_list) 默认行优先
+        # 所以这里先以 行优先 把 “h5 行优先 读进来的数据” 转成一维， 再以 列优先 转成 grid 对应的维度
+        if task.lower() == "rho":
+            if key is None:
+                _key = "/Rho/TotalCharge"
+            else:
+                _key = f"/Rho/{key}"
+        elif task.lower() == "potential":
+            if key is None:
+                _key = "/Potential/TotalElectrostaticPotential"
+            else:
+                _key = f"/Potential/{key}"
+        elif task.lower() == "elf":
+            if key is None:
+                _key = "/ELF/TotalELF"
+            else:
+                _key = f"/ELF/{key}"
+        elif task.lower() == "pcharge":
+            if key is None:
+                _key = "/Pcharge/1/TotalCharge"
+            else:
+                _key = f"/Pcharge/1/{key}"
+        elif task.lower() == "boundcharge":
+            if key is None:
+                _key = "/Rho"
+            else:
+                _key = key
+
+        if _key not in hdict:
+            raise KeyError(f"未找到{_key}键！")
+        tmp_pot = np.asarray(hdict[_key]).reshape([-1, 1], order="C")
+        ys = tmp_pot.reshape(grid, order="F")
+
+    elif datafile.endswith(".json"):
+        jfile = datafile
+        with open(jfile, "r") as f:
+            jdict = json.load(f)
+        grid = jdict["AtomInfo"]["Grid"]
+
+        if task.lower() == "rho":
+            if key is None:
+                ys = np.asarray(jdict["Rho"]["TotalCharge"]).reshape(grid, order="F")
+            else:
+                ys = np.asarray(jdict["Rho"][key]).reshape(grid, order="F")
+        elif task.lower() == "potential":
+            if key is None:
+                ys = np.asarray(
+                    jdict["Potential"]["TotalElectrostaticPotential"]
+                ).reshape(grid, order="F")
+            else:
+                ys = np.asarray(jdict["Potential"][key]).reshape(grid, order="F")
+        elif task.lower() == "elf":
+            if key is None:
+                ys = np.asarray(jdict["ELF"]["TotalELF"]).reshape(grid, order="F")
+            else:
+                ys = np.asarray(jdict["ELF"][key]).reshape(grid, order="F")
+        elif task.lower() == "pcharge":
+            if key is None:
+                ys = np.asarray(jdict["Pcharge"][0]["TotalCharge"]).reshape(
+                    grid, order="F"
+                )
+            else:
+                ys = np.asarray(jdict["Pcharge"][0][key]).reshape(grid, order="F")
+        else:
+            if key is None:
+                ys = np.asarray(jdict["Rho"]).reshape(grid, order="F")
+            else:
+                ys = np.asarray(jdict[key]).reshape(grid, order="F")
+
+    else:
+        raise TypeError("仅支持读取h5或json文件或直接传入数组！")
+
+    all_axis = [0, 1, 2]
+    all_axis.remove(axis)
+    y = np.mean(ys, tuple(all_axis))
+    x = np.arange(len(y))
+
+    if raw:
+        pd.DataFrame({"x": x, "y": y}).to_csv(f"raw{task}_axis{axis}.csv", index=False)
+    if smooth:
+        s = sm.nonparametric.lowess(y, x, frac=smooth_frac)
+        if raw:
+            pd.DataFrame({"x": s[:, 0], "y": s[:, 1]}).to_csv(
+                f"raw{task}_axis{axis}_smooth.csv", index=False
+            )
+
+        plt.plot(s[:, 0], s[:, 1], label="macroscopic average", **kwargs)
+
+    plt.plot(x, y, **kwargs)
+
+    return plt
+
+
+def plot_aimd(
+    datafile: str = "aimd.h5",
+    show: bool = True,
+    figname: str = "aimd.png",
+    flags_str="12345",
+    raw=False,
+):
+    r"""AIMD任务完成后，绘制关键物理量的收敛过程图
+
+    aimd.h5 -> aimd.png
+
+    Parameters
+    ----------
+    datafile : str or list
+        h5文件位置. 例如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
+    show : bool
+        是否展示交互界面. 默认 False
+    figname : str
+        保存的图片路径. 默认 'aimd.h5'
+    flags_str : str
+        子图编号.
+        1. 动能
+        2. 总能
+        3. 压力
+        4. 温度
+        5. 体积
+    raw : bool
+        是否输出原始数据到csv文件
+
+    Returns
+    ----------
+    figname : str
+        图片路径，默认 'aimd.png'
+
+    Examples
+    ----------
+    >>> from dspawpy.plot import plot_aimd
+
+    读取 aimd.h5 文件内容，画出动能、总能、温度、体积的收敛过程图，并保存相应数据到 rawaimd_*.csv 中
+
+    >>> plot_aimd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', flags_str='1245', raw=False, show=False, figname=None)
+    正在处理子图1
+     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    正在处理子图2
+     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    正在处理子图4
+     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    正在处理子图5
+     reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    """
+    # 处理用户读取，按顺序去重
+    temp = set()
+    flags = [x for x in flags_str if x not in temp and (temp.add(x) or True)]
+    if " " in flags:  # remove space
+        flags.remove(" ")
+
+    for flag in flags:
+        assert flag in ["1", "2", "3", "4", "5"], "读取错误！"
+
+    # 开始画组合图
+    N_figs = len(flags)
+    fig, axes = plt.subplots(N_figs, 1, sharex=True, figsize=(6, 2 * N_figs))
+    if N_figs == 1:  # 'AxesSubplot' object is not subscriptable
+        axes = [axes]  # 避免上述类型错误
+    fig.suptitle("DSPAW AIMD")
+    for i, flag in enumerate(flags):
+        print("正在处理子图" + flag)
+        # 读取数据
+        xs, ys = _read_aimd_converge_data(datafile, flag)
+        if raw:
+            pd.DataFrame({"x": xs, "y": ys}).to_csv(f"rawaimd_{flag}.csv", index=False)
+
+        axes[i].plot(xs, ys)  # 绘制坐标点
+        # 子图的y轴标签
+        if flag == "1":
+            axes[i].set_ylabel("Kinetic Energy (eV)")
+        elif flag == "2":
+            axes[i].set_ylabel("Energy (eV)")
+        elif flag == "3":
+            axes[i].set_ylabel("Pressure Kinetic (kbar)")
+        elif flag == "4":
+            axes[i].set_ylabel("Temperature (K)")
+        else:
+            axes[i].set_ylabel("Volume (Angstrom^3)")
+
+    plt.tight_layout()
+    # save and show
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
+    if show:
+        plt.show()
+
+
+def plot_bandunfolding(
+    datafile: str = "band.h5", ef=0.0, de=0.05, dele=0.06, raw=False
+):
+    r"""能带反折叠任务完成后，读取 h5 或 json 文件数据绘图
+
+    band.h5/band.json -> bandunfolding.png
+
+    Parameters
+    ----------
+    datafile : str
+        h5或json文件路径或包含任意这些文件的文件夹，默认 'band.h5'
+    ef : float
+        费米能级，默认置于 y = 0 处
+    de : float
+        能带宽度，默认0.05
+    dele : float
+        能带间隔，默认0.06
+    raw : bool
+        是否输出原始数据到rawbandunfolding.csv
+
+    Returns
+    -------
+    axes: matplotlib.axes._subplots.AxesSubplot
+        可传递给其他函数进行进一步处理
+
+    Examples
+    --------
+
+    绘图并保存原始数据到rawbandunfolding.csv
+
+    >>> from dspawpy.plot import plot_bandunfolding
+    >>> plot_bandunfolding("/data/home/hzw1002/dspawpy_repo/test/2.22/band.h5", raw=True)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.22/band.h5...
+    <module 'matplotlib.pyplot' from '/data/home/hzw1002/anaconda3/lib/python3.9/site-packages/matplotlib/pyplot.py'>
+    """
+    # search datafile in the given directory
+    if os.path.isdir(datafile):
+        directory = datafile  # specified datafile is actually a directory
+        print("您指定了一个文件夹，正在查找相关h5或json文件...")
+        if os.path.exists(os.path.join(directory, "band.h5")):
+            datafile = os.path.join(directory, "band.h5")
+            print("Reading band.h5...")
+        elif os.path.exists(os.path.join(directory, "band.json")):
+            datafile = os.path.join(directory, "band.json")
+            print("Reading band.json...")
+        else:
+            raise FileNotFoundError("未找到band.h5/band.json文件！")
+
+    if datafile.endswith(".h5"):
+        # band = load_h5(datafile)
+        import h5py
+
+        print(f"Reading {os.path.abspath(datafile)}...")
+        f = h5py.File(datafile, "r")
+        number_of_band = np.array(f["/BandInfo/NumberOfBand"])[0]
+        # number_of_band = band["/BandInfo/NumberOfBand"][0]
+        number_of_kpoints = np.array(f["/BandInfo/NumberOfKpoints"])[0]
+        # number_of_kpoints = band["/BandInfo/NumberOfKpoints"][0]
+        data = np.array(f["/UnfoldingBandInfo/Spin1/UnfoldingBand"])
+        # data = band["/UnfoldingBandInfo/Spin1/UnfoldingBand"]
+        weight = np.array(f["/UnfoldingBandInfo/Spin1/Weight"])
+        # weight = band["/UnfoldingBandInfo/Spin1/Weight"]
+    elif datafile.endswith(".json"):
+        with open(datafile, "r") as f:
+            band = json.load(f)
+        number_of_band = band["BandInfo"]["NumberOfBand"]
+        number_of_kpoints = band["BandInfo"]["NumberOfKpoints"]
+        data = band["UnfoldingBandInfo"]["Spin1"]["UnfoldingBand"]
+        weight = band["UnfoldingBandInfo"]["Spin1"]["Weight"]
+    else:
+        raise TypeError("仅支持读取h5或json文件！")
+
+    celtot = np.array(data).reshape((number_of_kpoints, number_of_band)).T
+    proj_wt = np.array(weight).reshape((number_of_kpoints, number_of_band)).T
+    X2, Y2, Z2, emin = getEwtData(
+        number_of_kpoints, number_of_band, celtot, proj_wt, ef, de, dele
+    )
+
+    if raw:
+        pd.DataFrame({"Y": Y2, "Z": Z2}, index=X2).to_csv(
+            "rawbandunfolding.csv", header=["Y", "color"], index=True, index_label="X"
+        )
+
+    plt.clf()
+    plt.scatter(X2, Y2, c=Z2, cmap="hot")
+    plt.xlim(0, 200)
+    plt.ylim(emin - 0.5, 15)
+    ax = plt.gca()
+    plt.colorbar()
+    ax.set_facecolor("black")
+
+    return plt
+
+
+def plot_optical(
+    datafile: str = "optical.h5",
+    key: str = "AbsorptionCoefficient",
+    index: int = 0,
+    raw=False,
+):
+    """光学性质计算任务完成后，读取数据并绘制预览图
+
+    optical.h5/optical.json -> optical.png
+
+    Parameters
+    ----------
+    datafile : str
+        h5或json文件路径或包含任意这些文件的文件夹，默认 'optical.h5'
+    key: str
+        可选 "AbsorptionCoefficient", "ExtinctionCoefficient", "RefractiveIndex", "Reflectance" 中的任意一个，默认 "AbsorptionCoefficient"
+    index : int
+        序号，默认0
+    raw : bool
+        是否保存原始数据到csv
+
+    Returns
+    -------
+    axes: matplotlib.axes._subplots.AxesSubplot
+        可传递给其他函数进行进一步处理
+
+    Examples
+    --------
+
+    绘图并保存原始数据到rawoptical.csv
+
+    >>> from dspawpy.plot import plot_optical
+    >>> plot_optical("/data/home/hzw1002/dspawpy_repo/test/2.12/scf.h5", "AbsorptionCoefficient", 0, raw=True)
+    >>> plot_optical("/data/home/hzw1002/dspawpy_repo/test/2.12/optical.json", "AbsorptionCoefficient", 0, raw=True)
+    """
+    # search datafile in the given directory
+    if os.path.isdir(datafile):
+        directory = datafile  # specified datafile is actually a directory
+        print("您指定了一个文件夹，正在查找相关h5或json文件...")
+        if os.path.exists(os.path.join(directory, "optical.h5")):
+            datafile = os.path.join(directory, "optical.h5")
+            print("Reading optical.h5...")
+        elif os.path.exists(os.path.join(directory, "optical.json")):
+            datafile = os.path.join(directory, "optical.json")
+            print("Reading optical.json...")
+        else:
+            raise FileNotFoundError("未找到optical.h5/optical.json文件！")
+
+    # parse the real datafile
+    if datafile.endswith("h5"):
+        data_all = load_h5(datafile)
+        energy = data_all["/OpticalInfo/EnergyAxe"]
+        data = data_all["/OpticalInfo/" + key]
+    elif datafile.endswith("json"):
+        with open(datafile, "r") as fin:
+            data_all = json.load(fin)
+        energy = data_all["OpticalInfo"]["EnergyAxe"]
+        data = data_all["OpticalInfo"][key]
+    else:
+        raise TypeError("仅支持读取h5或json文件！")
+
+    data = np.asarray(data).reshape(len(energy), 6)[:, index]
+    inter_f = interp1d(energy, data, kind="cubic")
+    energy_spline = np.linspace(energy[0], energy[-1], 2001)
+    data_spline = inter_f(energy_spline)
+
+    if raw:
+        pd.DataFrame({"energy": energy, "data": data}).to_csv(
+            "rawoptical.csv", index=False
+        )
+        pd.DataFrame(
+            {"energy_spline": energy_spline, "data_spline": data_spline}
+        ).to_csv("rawoptical_spline.csv", index=False)
+
+    plt.plot(energy_spline, data_spline, c="b")
+    plt.xlabel("Photon energy (eV)")
+    plt.ylabel("%s %s" % (key, r"$\alpha (\omega )(cm^{-1})$"))
+
+
+def plot_phonon_thermal(
+    datafile: str = "phonon.h5",
+    figname: str = "phonon.png",
+    show: bool = True,
+    raw=False,
+):
+    """声子热力学计算任务完成后，绘制相关物理量随温度变化曲线
+
+    phonon.h5/phonon.json -> phonon.png
+
+    Parameters
+    ----------
+    datafile : str
+        h5或json文件路径或包含任意这些文件的文件夹，默认 'phonon.h5'
+    figname : str
+        保存图片的文件名
+    show : bool
+        是否弹出交互界面
+    raw : bool
+        是否保存原始数据到rawphonon.csv文件
+
+    Returns
+    ----------
+    figname : str
+        图片路径，默认 'phonon.png'
+
+    Examples
+    --------
+    >>> from dspawpy.plot import plot_phonon_thermal
+    >>> plot_phonon_thermal('/data/home/hzw1002/dspawpy_repo/test/2.26/phonon.h5', figname='/data/home/hzw1002/dspawpy_repo/test/out/phonon_thermal.png', show=False)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.26/phonon.h5...
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/out/phonon_thermal.png
+    """
+    # search datafile in the given directory
+    if os.path.isdir(datafile):
+        directory = datafile  # specified datafile is actually a directory
+        print("您指定了一个文件夹，正在查找相关h5或json文件...")
+        if os.path.exists(os.path.join(directory, "phonon.h5")):
+            datafile = os.path.join(directory, "phonon.h5")
+            print("Reading phonon.h5...")
+        elif os.path.exists(os.path.join(directory, "phonon.json")):
+            datafile = os.path.join(directory, "phonon.json")
+            print("Reading phonon.json...")
+        else:
+            raise FileNotFoundError("未找到phonon.h5/phonon.json文件！")
+
+    if datafile.endswith(".h5"):
+        hfile = datafile
+        ph = h5py.File(hfile, "r")
+        print(f"Reading {hfile}...")
+        if "/ThermalInfo/Temperatures" not in ph:
+            raise KeyError(
+                "❓ No thermal info in datafile, you probably gave a wrong phonon.h5 file"
+            )
+        temp = np.array(ph["/ThermalInfo/Temperatures"])
+        entropy = np.array(ph["/ThermalInfo/Entropy"])
+        heat_capacity = np.array(ph["/ThermalInfo/HeatCapacity"])
+        helmholts_free_energy = np.array(ph["/ThermalInfo/HelmholtzFreeEnergy"])
+    elif datafile.endswith(".json"):
+        jfile = datafile
+        with open(jfile, "r") as f:
+            data = json.load(f)
+        print(f"Reading {jfile}...")
+        temp = np.array(data["ThermalInfo"]["Temperatures"])
+        entropy = np.array(data["ThermalInfo"]["Entropy"])
+        heat_capacity = np.array(data["ThermalInfo"]["HeatCapacity"])
+        helmholts_free_energy = np.array(data["ThermalInfo"]["HelmholtzFreeEnergy"])
+    else:
+        raise TypeError("仅支持读取h5或json文件！")
+
+    if raw:
+        pd.DataFrame(
+            {
+                "temp": temp,
+                "entropy": entropy,
+                "heat_capacity": heat_capacity,
+                "helmholts_free_energy": helmholts_free_energy,
+            }
+        ).to_csv("rawphonon.csv", index=False)
+
+    plt.plot(temp, entropy, c="red", label="Entropy (J/K/mol)")
+    plt.plot(temp, heat_capacity, c="green", label="Heat Capacity (J/K/mol)")
+    plt.plot(
+        temp, helmholts_free_energy, c="blue", label="Helmholtz Free Energy (kJ/mol)"
+    )
+    plt.xlabel("Temperature(K)")
+    plt.ylabel("Thermal Properties")
+    plt.tick_params(direction="in")  # 刻度线朝内
+    plt.grid(alpha=0.2)
+    plt.legend()
+    plt.title("Thermal")
+
+    plt.tight_layout()
+    # save and show
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
+    if show:
+        plt.show()
+
+
+def plot_polarization_figure(
+    directory: str,
+    repetition: int = 2,
+    annotation: bool = False,
+    annotation_style: int = 1,
+    show: bool = True,
+    figname: str = "pol.png",
+    raw=False,
+):
+    """绘制铁电极化结果图
+
+    Parameters
+    ----------
+    directory : str
+        铁电极化计算任务主目录
+    repetition : int
+        沿上（或下）方向重复绘制的次数, 默认 2
+    annotation : bool
+        是否显示首尾构型的铁电极化数值, 默认显示
+    show : bool
+        是否交互显示图片, 默认 True
+    figname : str
+        图片保存路径, 默认 'pol.png'
+    raw : bool
+        是否将原始数据保存到csv文件
+
+    Returns
+    -------
+    axes: matplotlib.axes._subplots.AxesSubplot
+        可传递给其他函数进行进一步处理
+
+    Examples
+    --------
+    >>> from dspawpy.plot import plot_polarization_figure
+    >>> plot_polarization_figure(directory='/data/home/hzw1002/dspawpy_repo/test/2.20', figname='/data/home/hzw1002/dspawpy_repo/test/out/pol.png', show=False)
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/out/pol.png
+    array([<Axes: title={'center': 'Px'}>, <Axes: title={'center': 'Py'}>,
+           <Axes: title={'center': 'Pz'}>], dtype=object)
+    """
+    assert repetition >= 0, "重复次数必须是自然数"
+    subfolders, quantum, totals = _get_subfolders_quantum_totals(directory)
+    number_sfs = [int(sf) for sf in subfolders]
+    fig, axes = plt.subplots(1, 3, sharey=True)
+    xyz = ["x", "y", "z"]
+    for j in range(3):  # x, y, z
+        ys = np.empty(shape=(len(subfolders), repetition * 2 + 1))
+        for r in range(repetition + 1):
+            ys[:, repetition - r] = totals[:, j] - quantum[j] * r
+            ys[:, repetition + r] = totals[:, j] + quantum[j] * r
+
+        axes[j].plot(number_sfs, ys, ".")  # plot
+        axes[j].set_title("P%s" % xyz[j])
+        axes[j].xaxis.set_ticks(number_sfs)  # 设置x轴刻度
+        axes[j].set_xticklabels(labels=subfolders, rotation=90)
+        axes[j].grid(axis="x", color="gray", linestyle=":", linewidth=0.5)
+        axes[j].tick_params(direction="in")
+        # set y ticks using the first and last values
+        if annotation:
+            if annotation_style == 2:
+                style = "arc,angleA=-0,angleB=0,armA=-10,armB=0,rad=0"
+                for i in range(repetition * 2 + 1):
+                    axes[j].annotate(
+                        f"{ys[0,i]:.2f}",
+                        xy=(number_sfs[0], ys[0, i]),
+                        xycoords="data",
+                        xytext=(number_sfs[-1] + 2, ys[0, i] - 8),
+                        textcoords="data",
+                        arrowprops=dict(
+                            arrowstyle="->",
+                            color="black",
+                            linewidth=0.75,
+                            shrinkA=2,
+                            shrinkB=1,
+                            connectionstyle=style,
+                        ),
+                    )
+                    axes[j].annotate(
+                        f"{ys[-1,i]:.2f}",
+                        xy=(number_sfs[-1], ys[-1, i]),
+                        xycoords="data",
+                        xytext=(number_sfs[-1] + 2, ys[-1, i] + 8),
+                        textcoords="data",
+                        arrowprops=dict(
+                            arrowstyle="->",
+                            color="black",
+                            linewidth=0.75,
+                            shrinkA=2,
+                            shrinkB=1,
+                            connectionstyle=style,
+                        ),
+                    )
+            elif annotation_style == 1:
+                for i in range(repetition * 2 + 1):
+                    axes[j].annotate(
+                        text=f"{ys[0,i]:.2f}",
+                        xy=(0, ys[0, i]),
+                        xytext=(0, ys[0, i] - np.max(ys) / repetition / 5),
+                    )
+                    axes[j].annotate(
+                        text=f"{ys[-1,i]:.2f}",
+                        xy=(len(subfolders) - 1, ys[-1, i]),
+                        xytext=(
+                            len(subfolders) - 1,
+                            ys[-1, i] - np.max(ys) / repetition / 5,
+                        ),
+                    )
+            else:
+                raise ValueError("annotation_style must be 1 or 2")
+
+        if raw:
+            pd.DataFrame(ys, index=subfolders).to_csv(f"pol_{xyz[j]}.csv")
+
+    plt.tight_layout()
+    # save and show
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
+    if show:
+        plt.show()
+
+    return axes
+
+
+def _get_subfolders_quantum_totals(directory: str):
+    """返回铁电极化计算任务的子目录、量子数、极化总量；
+
+    请勿创建其他子目录，否则会被错误读取
+
+    Parameters
+    ----------
+    directory：str
+        铁电极化计算任务主目录
+
+    Returns
+    -------
+    subfolders : list
+        子目录列表
+    quantum : np.ndarray
+        量子数，xyz三个方向, shape=(1, 3)
+    totals : np.ndarray
+        极化总量，xyz三个方向, shape=(len(subfolders), 3)
+    """
+
+    raw_subfolders = next(os.walk(directory))[1]
+    subfolders = []
+    for subfolder in raw_subfolders:
+        assert (
+            0 <= int(subfolder) < 100
+        ), f"--> You should rename subfolders to 0~99, but {subfolder} found"
+        try:
+            assert 0 <= int(subfolder) < 100
+            subfolders.append(subfolder)
+        except:
+            pass
+    subfolders.sort()  # 从小到大排序
+    if os.path.exists(f"{os.path.join(directory, subfolders[0])}/scf.h5"):
+        # quantum number if constant across the whole calculation,
+        # so, read only once
+        quantum = np.array(
+            h5py.File(f"{os.path.join(directory, subfolders[0])}/scf.h5").get(
+                "/PolarizationInfo/Quantum"
+            )
+        )
+        # the Total number is not constant
+        totals = np.empty(shape=(len(subfolders), 3))
+        for i, fd in enumerate(subfolders):
+            data = h5py.File(f"{os.path.join(directory, fd)}/scf.h5")
+            total = np.array(data.get("/PolarizationInfo/Total"))
+            totals[i] = total
+
+    elif os.path.exists(f"{os.path.join(directory, subfolders[0])}/polarization.json"):
+        # quantum number if constant across the whole calculation,
+        # so, read only once
+        with open(
+            f"{os.path.join(directory, subfolders[0])}/polarization.json", "r"
+        ) as f:
+            quantum = json.load(f)["PolarizationInfo"]["Quantum"]
+        # the Total number is not constant
+        totals = np.empty(shape=(len(subfolders), 3))
+        for i, fd in enumerate(subfolders):
+            with open(f"{os.path.join(directory, fd)}/polarization.json", "r") as f:
+                data = json.load(f)
+            total = data["PolarizationInfo"]["Total"]
+            totals[i] = np.array(total, dtype=float)
+
+    else:
+        raise ValueError("no polarization.json or scf.h5 file found")
+
+    return subfolders, quantum, totals
+
+
+def getEwtData(nk, nb, celtot, proj_wt, ef, de, dele):
+    emin = np.min(celtot) - de
+    emax = np.max(celtot) - de
+
+    emin = np.floor(emin - 0.2)
+    emax = max(np.ceil(emax) * 1.0, 5.0)
+
+    nps = int((emax - emin) / de)
+
+    X = np.zeros((nps + 1, nk))
+    Y = np.zeros((nps + 1, nk))
+
+    X2 = []
+    Y2 = []
+    Z2 = []
+
+    for ik in range(nk):
+        for ip in range(nps + 1):
+            omega = ip * de + emin + ef
+            X[ip][ik] = ik
+            Y[ip][ik] = ip * de + emin
+            ewts_value = 0
+            for ib in range(nb):
+                smearing = dele / np.pi / ((omega - celtot[ib][ik]) ** 2 + dele**2)
+                ewts_value += smearing * proj_wt[ib][ik]
+            if ewts_value > 0.01:
+                X2.append(ik)
+                Y2.append(ip * de + emin)
+                Z2.append(ewts_value)
+
+    Z2_half = max(Z2) / 2
+
+    for i, x in enumerate(Z2):
+        if x > Z2_half:
+            Z2[i] = Z2_half
+
+    return X2, Y2, Z2, emin
+
+
+def _read_aimd_converge_data(datafile: str, index: str = None):
+    """从datafile指定的路径读取index指定的数据，返回绘图用的xs和ys两个数组
+
+    Parameters
+    ----------
+    datafile : str or list
+        hdf5文件路径，如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
+    index : str
+        编号, 默认 None
+
+    Returns
+    -------
+    xs : np.ndarray
+        x轴数据
+    ys : np.ndarray
+        y轴数据
+    """
+    if isinstance(datafile, list):
+        xs = []
+        ys = []
+        for i, df in enumerate(datafile):
+            # concentrate returned np.ndarray
+            x, y = _read_aimd_converge_data(df, index)
+            xs.extend(x)
+            ys.extend(y)
+        xs = np.linspace(1, len(xs), len(xs))
+        return xs, ys
+
+    # search datafile in the given directory
+    elif isinstance(datafile, str):
+        if os.path.isdir(datafile):  # 如果是文件夹
+            directory = datafile  # specified datafile is actually a directory
+            print(f"您指定了一个文件夹，正在{directory}中自动查找aimd.h5...")
+            if os.path.exists(os.path.join(directory, "aimd.h5")):
+                datafile = os.path.join(directory, "aimd.h5")
+                print("Reading aimd.h5...")
+            else:
+                raise FileNotFoundError("未找到aimd.h5文件！")
+
+        elif datafile.endswith(".h5"):  # 如果是h5文件
+            hf = h5py.File(datafile)  # 加载h5文件
+            print(f" reading {os.path.abspath(datafile)}...")
+            Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
+            ys = np.empty(Nstep)  # 准备一个空数组
+            # 开始读取
+            if index == "5":
+                for i in range(1, Nstep + 1):
+                    ys[i - 1] = np.linalg.det(hf.get("/Structures/Step-%d/Lattice" % i))
+            else:
+                map = {
+                    "1": "IonsKineticEnergy",
+                    "2": "TotalEnergy0",
+                    "3": "PressureKinetic",
+                    "4": "Temperature",
+                }
+                for i in range(1, Nstep + 1):
+                    # 如果计算中断，则没有PressureKinetic这个键
+                    try:
+                        ys[i - 1] = np.array(
+                            hf.get("/AimdInfo/Step-%d/%s" % (i, map[index]))
+                        )
+                    except:
+                        ys[i - 1] = 0
+                        ys = np.delete(ys, -1)
+                        print(f"-> 计算中断于第 {Nstep} 步，未读取到第 {i} 步的 {map[index]} 数据！")
+                        break
+
+            Nstep = len(ys)  # 步数更新为实际完成的步数
+
+            # 返回xs，ys两个数组
+            return np.linspace(1, Nstep, Nstep), np.array(ys)
+
+        else:
+            raise TypeError("仅支持读取h5文件！")
+    else:
+        raise TypeError("datafile必须是字符串或列表！")
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -1,721 +1,721 @@
-# -*- coding: utf-8 -*-
-import os
-from typing import List, Union
-
-import matplotlib.pyplot as plt
-import numpy as np
-from pymatgen.core import Structure
-from scipy.ndimage import gaussian_filter1d
-
-from dspawpy.io.structure import build_Structures_from_datafile
-
-
-class MSD:
-    # 用于实际计算均方差的类，摘自pymatgen开源项目
-    def __init__(
-        self,
-        structures: List[Structure],
-        select: Union[str, List[int]] = "all",
-        msd_type="xyz",
-    ):
-        self.structures = structures
-        self.msd_type = msd_type
-
-        self.n_frames = len(structures)
-        if select == "all":
-            self.n_particles = len(structures[0])
-        else:
-            self.n_particles = len(select)
-        self.lattice = structures[0].lattice
-
-        self._parse_msd_type()
-
-        self._position_array = np.zeros((self.n_frames, self.n_particles, self.dim_fac))
-
-        if select == "all":
-            for i, s in enumerate(self.structures):
-                self._position_array[i, :, :] = s.frac_coords[:, self._dim]
-        else:
-            for i, s in enumerate(self.structures):
-                self._position_array[i, :, :] = s.frac_coords[select, :][:, self._dim]
-
-    def _parse_msd_type(self):
-        r"""Sets up the desired dimensionality of the MSD."""
-        keys = {
-            "x": [0],
-            "y": [1],
-            "z": [2],
-            "xy": [0, 1],
-            "xz": [0, 2],
-            "yz": [1, 2],
-            "xyz": [0, 1, 2],
-        }
-
-        self.msd_type = self.msd_type.lower()
-
-        try:
-            self._dim = keys[self.msd_type]
-        except KeyError:
-            raise ValueError(
-                "invalid msd_type: {} specified, please specify one of xyz, "
-                "xy, xz, yz, x, y, z".format(self.msd_type)
-            )
-
-        self.dim_fac = len(self._dim)
-
-    def run(self):
-        print("Calculating MSD...")
-        result = np.zeros((self.n_frames, self.n_particles))
-
-        rd = np.zeros((self.n_frames, self.n_particles, self.dim_fac))
-        for i in range(1, self.n_frames):
-            disp = self._position_array[i, :, :] - self._position_array[i - 1, :, :]
-            # mic by periodic boundary condition
-            disp[np.abs(disp) > 0.5] = disp[np.abs(disp) > 0.5] - np.sign(
-                disp[np.abs(disp) > 0.5]
-            )
-            disp = np.dot(disp, self.lattice.matrix)
-            rd[i, :, :] = disp
-        rd = np.cumsum(rd, axis=0)
-        for n in range(1, self.n_frames):
-            disp = rd[n:, :, :] - rd[:-n, :, :]  # [n:-n] window
-            sqdist = np.square(disp).sum(axis=-1)
-            result[n, :] = sqdist.mean(axis=0)
-
-        return result.mean(axis=1)
-
-
-class RDF:
-    # 用于快速计算径向分布函数的类
-    # Copyright (c) Materials Virtual Lab.
-    # Distributed under the terms of the BSD License.
-    def __init__(
-        self,
-        structures: Union[Structure, List[Structure]],
-        rmin: float = 0.0,
-        rmax: float = 10.0,
-        ngrid: float = 101,
-        sigma: float = 0.0,
-    ):
-        """This method calculates rdf on `np.linspace(rmin, rmax, ngrid)` points
-
-        Parameter
-        ---------
-        structures (list of pymatgen Structures): structures to compute RDF
-        rmin (float): minimal radius
-        rmax (float): maximal radius
-        ngrid (int): number of grid points, defaults to 101
-        sigma (float): smooth parameter
-        """
-        if isinstance(structures, Structure):
-            structures = [structures]
-        self.structures = structures
-        # Number of atoms in all structures should be the same
-        assert len({len(i) for i in self.structures}) == 1, "不同构型的原子数不等！"
-        elements = [[i.specie for i in j.sites] for j in self.structures]
-        unique_elements_on_sites = [len(set(i)) == 1 for i in list(zip(*elements))]
-
-        # For the same site index, all structures should have the same element there
-        if not all(unique_elements_on_sites):
-            raise RuntimeError("Elements are not the same at least for one site")
-
-        self.rmin = rmin
-        self.rmax = rmax
-        self.ngrid = ngrid
-
-        self.dr = (self.rmax - self.rmin) / (self.ngrid - 1)  # end points are on grid
-        self.r = np.linspace(self.rmin, self.rmax, self.ngrid)  # type: ignore
-        self.shell_volumes = 4.0 * np.pi * self.r**2 * self.dr
-        self.shell_volumes[self.shell_volumes < 1e-8] = 1e8  # avoid divide by zero
-
-        self.n_structures = len(self.structures)
-        self.sigma = np.ceil(sigma / self.dr)
-
-    def _dist_to_counts(self, d):
-        """Convert a distance array for counts in the bin
-
-        Parameter
-        ---------
-            d: (1D np.array)
-
-        Returns:
-            1D array of counts in the bins centered on self.r
-        """
-        counts = np.zeros((self.ngrid,))
-        indices = np.array(
-            np.floor((d - self.rmin + 0.5 * self.dr) / self.dr), dtype=int
-        )  # 将找到配对的距离转换为格点序号 (向下取整)
-        unique, val_counts = np.unique(indices, return_counts=True)
-        counts[unique] = val_counts
-        return counts
-
-    def get_rdf(
-        self,
-        ref_species: Union[str, List[str]],
-        species: Union[str, List[str]],
-        is_average=True,
-    ):
-        """Wrapper to get the rdf for a given species pair
-
-        Parameter
-        ---------
-        ref_species (list of species or just single specie str):
-            The reference species. The rdfs are calculated with these species at the center
-        species (list of species or just single specie str):
-            the species that we are interested in. The rdfs are calculated on these species.
-        is_average (bool):
-            whether to take the average over all structures
-
-        Returns
-        -------
-        (x, rdf)
-            x is the radial points, and rdf is the rdf value.
-        """
-        print("Calculating RDF...")
-        if isinstance(ref_species, str):
-            ref_species = [ref_species]
-
-        if isinstance(species, str):
-            species = [species]
-        ref_species_index = []
-        species_index = []
-        for i in range(len(self.structures[0].species)):
-            ele = str(self.structures[0].species[i])
-            if ele in ref_species:
-                ref_species_index.append(i)
-            if (
-                ele in species
-            ):  # @syyl use if instead of elif in case of `species = ref_species`
-                species_index.append(i)
-        all_rdfs = [
-            self.get_one_rdf(ref_species_index, species_index, i)[1]
-            for i in range(self.n_structures)
-        ]
-        if is_average:
-            all_rdfs = np.mean(all_rdfs, axis=0)
-        return self.r, all_rdfs
-
-    def get_one_rdf(
-        self,
-        ref_species_index: Union[str, List[str]],
-        species_index: Union[str, List[str]],
-        index=0,
-    ):
-        """Get the RDF for one structure, indicated by the index of the structure
-        in all structures"""
-        lattice = self.structures[index].lattice
-        distances = []
-        refsp_frac_coord = self.structures[index].frac_coords[ref_species_index]
-        sp_frac_coord = self.structures[index].frac_coords[species_index]
-        d = lattice.get_all_distances(refsp_frac_coord, sp_frac_coord)
-        indices = (
-            (d >= self.rmin - self.dr / 2.0)
-            & (d <= self.rmax + self.dr / 2.0)
-            & (d > 1e-8)
-        )
-        distances = d[indices]
-        counts = self._dist_to_counts(np.array(distances))  # 统计该距离内目标元素的原子数，列表
-
-        npairs = len(distances)
-        rdf_temp = counts / npairs / self.shell_volumes / self.structures[index].volume
-
-        if self.sigma > 1e-8:
-            rdf_temp = gaussian_filter1d(rdf_temp, self.sigma)
-        return self.r, rdf_temp, npairs
-
-    def get_coordination_number(self, ref_species, species, is_average=True):
-        """returns running coordination number
-
-        Parameter
-        ---------
-        ref_species (list of species or just single specie str):
-            the reference species. The rdfs are calculated with these species at the center
-        species (list of species or just single specie str):
-            the species that we are interested in. The rdfs are calculated on these species.
-        is_average (bool): whether to take structural average
-
-        Returns
-        --------
-        numpy array
-        """
-        print("Calculating coordination number...")
-        # Note: The average density from all input structures is used here.
-        all_rdf = self.get_rdf(ref_species, species, is_average=False)[1]
-        if isinstance(species, str):
-            species = [species]
-        density = [sum(i[j] for j in species) for i in self.density]
-        cn = [
-            np.cumsum(rdf * density[i] * 4.0 * np.pi * self.r**2 * self.dr)
-            for i, rdf in enumerate(all_rdf)
-        ]
-        if is_average:
-            cn = np.mean(cn, axis=0)
-        return self.r, cn
-
-
-class RMSD:
-    # 用于计算均方差根（Root Mean Square Deviation）的类，摘自pymatgen开源项目
-    def __init__(self, structures: List[Structure]):
-        self.structures = structures
-
-        self.n_frames = len(self.structures)
-        self.n_particles = len(self.structures[0])
-        self.lattice = self.structures[0].lattice
-
-        self._position_array = np.zeros((self.n_frames, self.n_particles, 3))
-
-        for i, s in enumerate(self.structures):
-            self._position_array[i, :, :] = s.frac_coords
-
-    def run(self, base_index=0):
-        print("Calculating RMSD...")
-        result = np.zeros(self.n_frames)
-        rd = np.zeros((self.n_frames, self.n_particles, 3))
-        for i in range(1, self.n_frames):
-            disp = self._position_array[i, :, :] - self._position_array[i - 1, :, :]
-            # mic by periodic boundary condition
-            disp[np.abs(disp) > 0.5] = disp[np.abs(disp) > 0.5] - np.sign(
-                disp[np.abs(disp) > 0.5]
-            )
-            disp = np.dot(disp, self.lattice.matrix)
-            rd[i, :, :] = disp
-        rd = np.cumsum(rd, axis=0)
-
-        for i in range(self.n_frames):
-            sqdist = np.square(rd[i] - rd[base_index]).sum(axis=-1)
-            result[i] = sqdist.mean()
-
-        return np.sqrt(result)
-
-
-def get_lagtime_msd(
-    datafile: Union[str, List[str]],
-    select: Union[str, List[int]] = "all",
-    msd_type: str = "xyz",
-    timestep: float = 1.0,
-):
-    r"""计算不同时间步长下的均方差
-
-    Parameters
-    ----------
-    datafile : str or list of str
-        aimd.h5或aimd.json文件或包含这两个文件之一的文件夹；
-        写成列表的话将依次读取数据并合并到一起
-    select : str or list of int
-        原子序号列表，原子序号从0开始编号；默认为'all'，计算所有原子
-        暂不支持计算多个元素的MSD
-    msd_type : str
-        计算MSD的类型，可选xyz,xy,xz,yz,x,y,z，默认为'xyz'，即计算所有分量
-    timestep : float
-        时间间隔，单位为fs，默认1.0fs
-
-    Returns
-    -------
-    lagtime : np.ndarray
-        时间序列
-    result : np.ndarray
-        均方差序列
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_msd
-    >>> lagtime, msd = get_lagtime_msd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5')
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    Calculating MSD...
-    >>> lagtime
-    array([0.000e+00, 1.000e+00, 2.000e+00, ..., 1.997e+03, 1.998e+03,
-           1.999e+03])
-    >>> msd
-    array([0.00000000e+00, 4.04296586e-02, 9.35606189e-02, ...,
-           6.47011135e+03, 6.47105880e+03, 6.47194457e+03])
-    """
-    strs = build_Structures_from_datafile(datafile)
-
-    msd = MSD(strs, select, msd_type)
-    result = msd.run()
-
-    nframes = msd.n_frames
-    lagtime = np.arange(nframes) * timestep  # make the lag-time axis
-
-    return lagtime, result
-
-
-def get_lagtime_rmsd(datafile: Union[str, List[str]], timestep: float = 1.0):
-    r"""
-
-    Parameters
-    ----------
-    datafile : str or list of str
-        aimd.h5或aimd.json文件或包含这两个文件之一的文件夹；
-        写成列表的话将依次读取数据并合并到一起
-    timestep : float
-        时间步长，单位fs，默认1fs
-
-    Returns
-    -------
-    lagtime : numpy.ndarray
-        时间序列
-    rmsd : numpy.ndarray
-        均方根序列
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd
-    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', timestep=0.1)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    Calculating RMSD...
-    >>> lagtime
-    array([0.000e+00, 1.000e-01, 2.000e-01, ..., 1.997e+02, 1.998e+02,
-           1.999e+02])
-    >>> rmsd
-    array([0.00000000e+00, 3.56025899e-02, 6.28159066e-02, ...,
-           8.04616858e+01, 8.04569185e+01, 8.04483969e+01])
-    """
-    strs = build_Structures_from_datafile(datafile)
-
-    rmsd = RMSD(structures=strs)
-    result = rmsd.run()
-
-    # Plot
-    nframes = rmsd.n_frames
-    lagtime = np.arange(nframes) * timestep  # make the lag-time axis
-
-    return lagtime, result
-
-
-def get_rs_rdfs(
-    datafile: Union[str, List[str]],
-    ele1: str,
-    ele2: str,
-    rmin: float = 0,
-    rmax: float = 10,
-    ngrid: float = 101,
-    sigma: float = 0,
-):
-    r"""计算rdf分布函数
-
-    Parameters
-    ----------
-    datafile : str or list of str
-        aimd.h5或aimd.json文件路径或包含这两个文件之一的文件夹；
-        写成列表的话将依次读取数据并合并到一起
-    ele1 : list
-        中心元素
-    ele2 : list
-        相邻元素
-    rmin : float
-        径向分布最小值，默认为0
-    rmax : float
-        径向分布最大值，默认为10
-    ngrid : int
-        径向分布网格数，默认为101
-    sigma : float
-        平滑参数
-
-    Returns
-    -------
-    r : numpy.ndarray
-        径向分布网格点
-    rdf : numpy.ndarray
-        径向分布函数
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_rs_rdfs
-    >>> rs, rdfs = get_rs_rdfs(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5',ele1='H',ele2='O')
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    Calculating RDF...
-    >>> rdfs
-    array([0.00000000e+00, 0.00000000e+00, 4.66650481e-04, 9.30940287e-04,
-           3.52585381e-04, 1.26407382e-03, 1.25318841e-03, 1.50559377e-03,
-           1.11044305e-03, 2.60362277e-03, 2.84955254e-03, 1.98326911e-03,
-           1.25972719e-03, 8.84132365e-04, 5.74489287e-04, 4.16191635e-04,
-           1.31901135e-04, 1.88536303e-04, 1.16355309e-04, 1.19347145e-04,
-           5.65480311e-05, 3.78209587e-05, 2.34431565e-05, 1.10925032e-05,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00])
-    """
-    strs = build_Structures_from_datafile(datafile)
-    # print(strs[0]) # check pbc
-    # raise ValueError
-
-    # 计算rdf并绘制主要曲线
-    obj = RDF(structures=strs, rmin=rmin, rmax=rmax, ngrid=ngrid, sigma=sigma)
-
-    rs, rdfs = obj.get_rdf(ele1, ele2)
-    return rs, rdfs
-
-
-def plot_msd(
-    lagtime: np.ndarray,
-    result: np.ndarray,
-    xlim: List[float] = None,
-    ylim: List[float] = None,
-    figname: str = None,
-    show: bool = True,
-    ax=None,
-    **kwargs,
-):
-    r"""AIMD任务完成后，计算均方差（MSD）
-
-    Parameters
-    ----------
-    lagtime : np.ndarray
-        时间序列
-    result : np.ndarray
-        均方差序列
-    xlim : list of float
-        x轴的范围，默认为None，自动设置
-    ylim : list of float
-        y轴的范围，默认为None，自动设置
-    figname : str
-        图片名称，默认为None，不保存图片
-    show : bool
-        是否显示图片，默认为True
-    ax: matplotlib axes object
-        用于将图片绘制到matplotlib的子图上
-    **kwargs : dict
-        其他参数，如线条宽度、颜色等，传递给plt.plot函数
-
-    Returns
-    -------
-    MSD分析后的图片
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_msd, plot_msd
-
-    指定h5文件位置，用 get_lagtime_msd 函数获取数据，select 参数选择第n个原子（不是元素）
-
-    >>> lagtime, msd = get_lagtime_msd('/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', select=[0])
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    Calculating MSD...
-
-    用获取的数据画图并保存
-
-    >>> plot_msd(lagtime, msd, figname='/data/home/hzw1002/dspawpy_repo/test/out/MSD.png', show=False)
-    MSD图片保存在 /data/home/hzw1002/dspawpy_repo/test/out/MSD.png
-    <Axes: xlabel='Time (fs)', ylabel='MSD (Å)'>
-    """
-    if ax:
-        ishow = False
-        ax.plot(lagtime, result, c="black", ls="-", **kwargs)
-    else:
-        ishow = True
-        fig, ax = plt.subplots()
-        ax.plot(lagtime, result, c="black", ls="-", **kwargs)
-        ax.set_xlabel("Time (fs)")
-        ax.set_ylabel("MSD (Å)")
-
-    if xlim:
-        ax.set_xlim(xlim)
-    if ylim:
-        ax.set_ylim(ylim)
-
-    plt.tight_layout()
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print("MSD图片保存在", os.path.abspath(figname))
-    if show and ishow:  # 画子图的话，不应每个子图都show
-        plt.show()  # show会自动清空图片
-
-    return ax
-
-
-def plot_rdf(
-    rs: np.ndarray,
-    rdfs: np.ndarray,
-    ele1: str,
-    ele2: str,
-    xlim: list = None,
-    ylim: list = None,
-    figname: str = None,
-    show: bool = True,
-    ax: plt.Axes = None,
-    **kwargs,
-):
-    r"""AIMD计算后分析rdf并画图
-
-    Parameters
-    ----------
-    rs : numpy.ndarray
-        径向分布网格点
-    rdfs : numpy.ndarray
-        径向分布函数
-    ele1 : list
-        中心元素
-    ele2 : list
-        相邻元素
-    xlim : list
-        x轴范围，默认为None，即自动设置
-    ylim : list
-        y轴范围，默认为None，即自动设置
-    figname : str
-        图片名称，默认为None，即不保存图片
-    show : bool
-        是否显示图片，默认为True
-    ax: matplotlib.axes.Axes
-        画图的坐标轴，默认为None，即新建坐标轴
-    **kwargs : dict
-        其他参数，如线条宽度、颜色等，传递给plt.plot函数
-
-    Returns
-    -------
-    rdf分析后的图片
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
-
-    先获取rs和rdfs数据作为xy轴数据
-
-    >>> rs, rdfs = get_rs_rdfs('/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', 'H', 'O', rmax=6)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    Calculating RDF...
-
-    将xy轴数据传入plot_rdf函数绘图
-
-    >>> plot_rdf(rs, rdfs, 'H','O', figname='/data/home/hzw1002/dspawpy_repo/test/out/RDF.png', show=False)
-    图片已保存到 /data/home/hzw1002/dspawpy_repo/test/out/RDF.png
-    """
-
-    if ax:
-        ishow = False
-        ax.plot(
-            rs,
-            rdfs,
-            label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
-            **kwargs,
-        )
-
-    else:
-        ishow = True
-        fig, ax = plt.subplots()
-        ax.plot(
-            rs,
-            rdfs,
-            label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
-            **kwargs,
-        )
-
-        ax.set_xlabel(r"$r$" + "(Å)")
-        ax.set_ylabel(r"$g(r)$")
-
-    ax.legend()
-
-    # 绘图细节
-    if xlim:
-        ax.set_xlim(xlim)
-    if ylim:
-        ax.set_ylim(ylim)
-
-    plt.tight_layout()
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"图片已保存到 {os.path.abspath(figname)}")
-    if show and ishow:  # 画子图的话，不应每个子图都show
-        plt.show()  # show会自动清空图片
-
-
-def plot_rmsd(
-    lagtime: np.ndarray,
-    result: np.ndarray,
-    xlim: list = None,
-    ylim: list = None,
-    figname: str = None,
-    show: bool = True,
-    ax=None,
-    **kwargs,
-):
-    r"""AIMD计算后分析rmsd并画图
-
-    Parameters
-    ----------
-    lagtime:
-        时间序列
-    result:
-        均方根序列
-    xlim : list
-        x轴范围
-    ylim : list
-        y轴范围
-    figname : str
-        图片保存路径
-    show : bool
-        是否显示图片
-    ax : matplotlib.axes._subplots.AxesSubplot
-        画子图的话，传入子图对象
-    **kwargs : dict
-        传入plt.plot的参数
-
-    Returns
-    -------
-    rmsd分析结构的图片
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
-
-    timestep 表示时间步长
-
-    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', timestep=0.1)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    Calculating RMSD...
-
-    直接保存为RMSD.png图片
-
-    >>> plot_rmsd(lagtime, rmsd, figname='/data/home/hzw1002/dspawpy_repo/test/out/RMSD.png', show=False)
-    图片已保存到 /data/home/hzw1002/dspawpy_repo/test/out/RMSD.png
-    <Axes: xlabel='Time (fs)', ylabel='RMSD (Å)'>
-    """
-    # 参数初始化
-    if not ax:
-        ishow = True
-    else:
-        ishow = False
-
-    if ax:
-        ax.plot(lagtime, result, **kwargs)
-    else:
-        fig, ax = plt.subplots()
-        ax.plot(lagtime, result, **kwargs)
-        ax.set_xlabel("Time (fs)")
-        ax.set_ylabel("RMSD (Å)")
-
-    if xlim:
-        ax.set_xlim(xlim)
-    if ylim:
-        ax.set_ylim(ylim)
-
-    plt.tight_layout()
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"图片已保存到 {os.path.abspath(figname)}")
-    if show and ishow:  # 画子图的话，不应每个子图都show
-        plt.show()  # show会自动清空图片
-
-    return ax
+# -*- coding: utf-8 -*-
+import os
+from typing import List, Union
+
+import matplotlib.pyplot as plt
+import numpy as np
+from pymatgen.core import Structure
+from scipy.ndimage import gaussian_filter1d
+
+from dspawpy.io.structure import build_Structures_from_datafile
+
+
+class MSD:
+    # 用于实际计算均方差的类，摘自pymatgen开源项目
+    def __init__(
+        self,
+        structures: List[Structure],
+        select: Union[str, List[int]] = "all",
+        msd_type="xyz",
+    ):
+        self.structures = structures
+        self.msd_type = msd_type
+
+        self.n_frames = len(structures)
+        if select == "all":
+            self.n_particles = len(structures[0])
+        else:
+            self.n_particles = len(select)
+        self.lattice = structures[0].lattice
+
+        self._parse_msd_type()
+
+        self._position_array = np.zeros((self.n_frames, self.n_particles, self.dim_fac))
+
+        if select == "all":
+            for i, s in enumerate(self.structures):
+                self._position_array[i, :, :] = s.frac_coords[:, self._dim]
+        else:
+            for i, s in enumerate(self.structures):
+                self._position_array[i, :, :] = s.frac_coords[select, :][:, self._dim]
+
+    def _parse_msd_type(self):
+        r"""Sets up the desired dimensionality of the MSD."""
+        keys = {
+            "x": [0],
+            "y": [1],
+            "z": [2],
+            "xy": [0, 1],
+            "xz": [0, 2],
+            "yz": [1, 2],
+            "xyz": [0, 1, 2],
+        }
+
+        self.msd_type = self.msd_type.lower()
+
+        try:
+            self._dim = keys[self.msd_type]
+        except KeyError:
+            raise ValueError(
+                "invalid msd_type: {} specified, please specify one of xyz, "
+                "xy, xz, yz, x, y, z".format(self.msd_type)
+            )
+
+        self.dim_fac = len(self._dim)
+
+    def run(self):
+        print("Calculating MSD...")
+        result = np.zeros((self.n_frames, self.n_particles))
+
+        rd = np.zeros((self.n_frames, self.n_particles, self.dim_fac))
+        for i in range(1, self.n_frames):
+            disp = self._position_array[i, :, :] - self._position_array[i - 1, :, :]
+            # mic by periodic boundary condition
+            disp[np.abs(disp) > 0.5] = disp[np.abs(disp) > 0.5] - np.sign(
+                disp[np.abs(disp) > 0.5]
+            )
+            disp = np.dot(disp, self.lattice.matrix)
+            rd[i, :, :] = disp
+        rd = np.cumsum(rd, axis=0)
+        for n in range(1, self.n_frames):
+            disp = rd[n:, :, :] - rd[:-n, :, :]  # [n:-n] window
+            sqdist = np.square(disp).sum(axis=-1)
+            result[n, :] = sqdist.mean(axis=0)
+
+        return result.mean(axis=1)
+
+
+class RDF:
+    # 用于快速计算径向分布函数的类
+    # Copyright (c) Materials Virtual Lab.
+    # Distributed under the terms of the BSD License.
+    def __init__(
+        self,
+        structures: Union[Structure, List[Structure]],
+        rmin: float = 0.0,
+        rmax: float = 10.0,
+        ngrid: float = 101,
+        sigma: float = 0.0,
+    ):
+        """This method calculates rdf on `np.linspace(rmin, rmax, ngrid)` points
+
+        Parameter
+        ---------
+        structures (list of pymatgen Structures): structures to compute RDF
+        rmin (float): minimal radius
+        rmax (float): maximal radius
+        ngrid (int): number of grid points, defaults to 101
+        sigma (float): smooth parameter
+        """
+        if isinstance(structures, Structure):
+            structures = [structures]
+        self.structures = structures
+        # Number of atoms in all structures should be the same
+        assert len({len(i) for i in self.structures}) == 1, "不同构型的原子数不等！"
+        elements = [[i.specie for i in j.sites] for j in self.structures]
+        unique_elements_on_sites = [len(set(i)) == 1 for i in list(zip(*elements))]
+
+        # For the same site index, all structures should have the same element there
+        if not all(unique_elements_on_sites):
+            raise RuntimeError("Elements are not the same at least for one site")
+
+        self.rmin = rmin
+        self.rmax = rmax
+        self.ngrid = ngrid
+
+        self.dr = (self.rmax - self.rmin) / (self.ngrid - 1)  # end points are on grid
+        self.r = np.linspace(self.rmin, self.rmax, self.ngrid)  # type: ignore
+        self.shell_volumes = 4.0 * np.pi * self.r**2 * self.dr
+        self.shell_volumes[self.shell_volumes < 1e-8] = 1e8  # avoid divide by zero
+
+        self.n_structures = len(self.structures)
+        self.sigma = np.ceil(sigma / self.dr)
+
+    def _dist_to_counts(self, d):
+        """Convert a distance array for counts in the bin
+
+        Parameter
+        ---------
+            d: (1D np.array)
+
+        Returns:
+            1D array of counts in the bins centered on self.r
+        """
+        counts = np.zeros((self.ngrid,))
+        indices = np.array(
+            np.floor((d - self.rmin + 0.5 * self.dr) / self.dr), dtype=int
+        )  # 将找到配对的距离转换为格点序号 (向下取整)
+        unique, val_counts = np.unique(indices, return_counts=True)
+        counts[unique] = val_counts
+        return counts
+
+    def get_rdf(
+        self,
+        ref_species: Union[str, List[str]],
+        species: Union[str, List[str]],
+        is_average=True,
+    ):
+        """Wrapper to get the rdf for a given species pair
+
+        Parameter
+        ---------
+        ref_species (list of species or just single specie str):
+            The reference species. The rdfs are calculated with these species at the center
+        species (list of species or just single specie str):
+            the species that we are interested in. The rdfs are calculated on these species.
+        is_average (bool):
+            whether to take the average over all structures
+
+        Returns
+        -------
+        (x, rdf)
+            x is the radial points, and rdf is the rdf value.
+        """
+        print("Calculating RDF...")
+        if isinstance(ref_species, str):
+            ref_species = [ref_species]
+
+        if isinstance(species, str):
+            species = [species]
+        ref_species_index = []
+        species_index = []
+        for i in range(len(self.structures[0].species)):
+            ele = str(self.structures[0].species[i])
+            if ele in ref_species:
+                ref_species_index.append(i)
+            if (
+                ele in species
+            ):  # @syyl use if instead of elif in case of `species = ref_species`
+                species_index.append(i)
+        all_rdfs = [
+            self.get_one_rdf(ref_species_index, species_index, i)[1]
+            for i in range(self.n_structures)
+        ]
+        if is_average:
+            all_rdfs = np.mean(all_rdfs, axis=0)
+        return self.r, all_rdfs
+
+    def get_one_rdf(
+        self,
+        ref_species_index: Union[str, List[str]],
+        species_index: Union[str, List[str]],
+        index=0,
+    ):
+        """Get the RDF for one structure, indicated by the index of the structure
+        in all structures"""
+        lattice = self.structures[index].lattice
+        distances = []
+        refsp_frac_coord = self.structures[index].frac_coords[ref_species_index]
+        sp_frac_coord = self.structures[index].frac_coords[species_index]
+        d = lattice.get_all_distances(refsp_frac_coord, sp_frac_coord)
+        indices = (
+            (d >= self.rmin - self.dr / 2.0)
+            & (d <= self.rmax + self.dr / 2.0)
+            & (d > 1e-8)
+        )
+        distances = d[indices]
+        counts = self._dist_to_counts(np.array(distances))  # 统计该距离内目标元素的原子数，列表
+
+        npairs = len(distances)
+        rdf_temp = counts / npairs / self.shell_volumes / self.structures[index].volume
+
+        if self.sigma > 1e-8:
+            rdf_temp = gaussian_filter1d(rdf_temp, self.sigma)
+        return self.r, rdf_temp, npairs
+
+    def get_coordination_number(self, ref_species, species, is_average=True):
+        """returns running coordination number
+
+        Parameter
+        ---------
+        ref_species (list of species or just single specie str):
+            the reference species. The rdfs are calculated with these species at the center
+        species (list of species or just single specie str):
+            the species that we are interested in. The rdfs are calculated on these species.
+        is_average (bool): whether to take structural average
+
+        Returns
+        --------
+        numpy array
+        """
+        print("Calculating coordination number...")
+        # Note: The average density from all input structures is used here.
+        all_rdf = self.get_rdf(ref_species, species, is_average=False)[1]
+        if isinstance(species, str):
+            species = [species]
+        density = [sum(i[j] for j in species) for i in self.density]
+        cn = [
+            np.cumsum(rdf * density[i] * 4.0 * np.pi * self.r**2 * self.dr)
+            for i, rdf in enumerate(all_rdf)
+        ]
+        if is_average:
+            cn = np.mean(cn, axis=0)
+        return self.r, cn
+
+
+class RMSD:
+    # 用于计算均方差根（Root Mean Square Deviation）的类，摘自pymatgen开源项目
+    def __init__(self, structures: List[Structure]):
+        self.structures = structures
+
+        self.n_frames = len(self.structures)
+        self.n_particles = len(self.structures[0])
+        self.lattice = self.structures[0].lattice
+
+        self._position_array = np.zeros((self.n_frames, self.n_particles, 3))
+
+        for i, s in enumerate(self.structures):
+            self._position_array[i, :, :] = s.frac_coords
+
+    def run(self, base_index=0):
+        print("Calculating RMSD...")
+        result = np.zeros(self.n_frames)
+        rd = np.zeros((self.n_frames, self.n_particles, 3))
+        for i in range(1, self.n_frames):
+            disp = self._position_array[i, :, :] - self._position_array[i - 1, :, :]
+            # mic by periodic boundary condition
+            disp[np.abs(disp) > 0.5] = disp[np.abs(disp) > 0.5] - np.sign(
+                disp[np.abs(disp) > 0.5]
+            )
+            disp = np.dot(disp, self.lattice.matrix)
+            rd[i, :, :] = disp
+        rd = np.cumsum(rd, axis=0)
+
+        for i in range(self.n_frames):
+            sqdist = np.square(rd[i] - rd[base_index]).sum(axis=-1)
+            result[i] = sqdist.mean()
+
+        return np.sqrt(result)
+
+
+def get_lagtime_msd(
+    datafile: Union[str, List[str]],
+    select: Union[str, List[int]] = "all",
+    msd_type: str = "xyz",
+    timestep: float = 1.0,
+):
+    r"""计算不同时间步长下的均方差
+
+    Parameters
+    ----------
+    datafile : str or list of str
+        aimd.h5或aimd.json文件或包含这两个文件之一的文件夹；
+        写成列表的话将依次读取数据并合并到一起
+    select : str or list of int
+        原子序号列表，原子序号从0开始编号；默认为'all'，计算所有原子
+        暂不支持计算多个元素的MSD
+    msd_type : str
+        计算MSD的类型，可选xyz,xy,xz,yz,x,y,z，默认为'xyz'，即计算所有分量
+    timestep : float
+        时间间隔，单位为fs，默认1.0fs
+
+    Returns
+    -------
+    lagtime : np.ndarray
+        时间序列
+    result : np.ndarray
+        均方差序列
+
+    Examples
+    --------
+    >>> from dspawpy.analysis.aimdtools import get_lagtime_msd
+    >>> lagtime, msd = get_lagtime_msd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5')
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    Calculating MSD...
+    >>> lagtime
+    array([0.000e+00, 1.000e+00, 2.000e+00, ..., 1.997e+03, 1.998e+03,
+           1.999e+03])
+    >>> msd
+    array([0.00000000e+00, 8.80447550e-02, 1.83768134e-01, ...,
+           9.66185452e+02, 9.66812755e+02, 9.67357702e+02])
+    """
+    strs = build_Structures_from_datafile(datafile)
+
+    msd = MSD(strs, select, msd_type)
+    result = msd.run()
+
+    nframes = msd.n_frames
+    lagtime = np.arange(nframes) * timestep  # make the lag-time axis
+
+    return lagtime, result
+
+
+def get_lagtime_rmsd(datafile: Union[str, List[str]], timestep: float = 1.0):
+    r"""
+
+    Parameters
+    ----------
+    datafile : str or list of str
+        aimd.h5或aimd.json文件或包含这两个文件之一的文件夹；
+        写成列表的话将依次读取数据并合并到一起
+    timestep : float
+        时间步长，单位fs，默认1fs
+
+    Returns
+    -------
+    lagtime : numpy.ndarray
+        时间序列
+    rmsd : numpy.ndarray
+        均方根序列
+
+    Examples
+    --------
+    >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd
+    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', timestep=0.1)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    Calculating RMSD...
+    >>> lagtime
+    array([0.000e+00, 1.000e-01, 2.000e-01, ..., 1.997e+02, 1.998e+02,
+           1.999e+02])
+    >>> rmsd
+    array([ 0.        ,  0.04849931,  0.09181907, ..., 31.09991413,
+           31.10077061, 31.10237454])
+    """
+    strs = build_Structures_from_datafile(datafile)
+
+    rmsd = RMSD(structures=strs)
+    result = rmsd.run()
+
+    # Plot
+    nframes = rmsd.n_frames
+    lagtime = np.arange(nframes) * timestep  # make the lag-time axis
+
+    return lagtime, result
+
+
+def get_rs_rdfs(
+    datafile: Union[str, List[str]],
+    ele1: str,
+    ele2: str,
+    rmin: float = 0,
+    rmax: float = 10,
+    ngrid: float = 101,
+    sigma: float = 0,
+):
+    r"""计算rdf分布函数
+
+    Parameters
+    ----------
+    datafile : str or list of str
+        aimd.h5或aimd.json文件路径或包含这两个文件之一的文件夹；
+        写成列表的话将依次读取数据并合并到一起
+    ele1 : list
+        中心元素
+    ele2 : list
+        相邻元素
+    rmin : float
+        径向分布最小值，默认为0
+    rmax : float
+        径向分布最大值，默认为10
+    ngrid : int
+        径向分布网格数，默认为101
+    sigma : float
+        平滑参数
+
+    Returns
+    -------
+    r : numpy.ndarray
+        径向分布网格点
+    rdf : numpy.ndarray
+        径向分布函数
+
+    Examples
+    --------
+    >>> from dspawpy.analysis.aimdtools import get_rs_rdfs
+    >>> rs, rdfs = get_rs_rdfs(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5',ele1='H',ele2='O')
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    Calculating RDF...
+    >>> rdfs
+    array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           6.90409153e-05, 7.47498606e-04, 2.40555636e-03, 2.57666881e-03,
+           2.53257125e-03, 2.37964722e-03, 1.80028135e-03, 1.20224160e-03,
+           7.57927477e-04, 3.41004760e-04, 2.85680407e-04, 1.72795412e-04,
+           1.49718401e-04, 1.44477999e-04, 2.23702566e-04, 2.11836218e-04,
+           1.34146448e-04, 1.78839343e-04, 9.16910363e-05, 1.45492991e-05,
+           3.70494493e-05, 3.72784113e-05, 2.82725837e-05, 3.19750004e-05,
+           8.46456322e-07, 4.72401470e-06, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00])
+    """
+    strs = build_Structures_from_datafile(datafile)
+    # print(strs[0]) # check pbc
+    # raise ValueError
+
+    # 计算rdf并绘制主要曲线
+    obj = RDF(structures=strs, rmin=rmin, rmax=rmax, ngrid=ngrid, sigma=sigma)
+
+    rs, rdfs = obj.get_rdf(ele1, ele2)
+    return rs, rdfs
+
+
+def plot_msd(
+    lagtime: np.ndarray,
+    result: np.ndarray,
+    xlim: List[float] = None,
+    ylim: List[float] = None,
+    figname: str = None,
+    show: bool = True,
+    ax=None,
+    **kwargs,
+):
+    r"""AIMD任务完成后，计算均方差（MSD）
+
+    Parameters
+    ----------
+    lagtime : np.ndarray
+        时间序列
+    result : np.ndarray
+        均方差序列
+    xlim : list of float
+        x轴的范围，默认为None，自动设置
+    ylim : list of float
+        y轴的范围，默认为None，自动设置
+    figname : str
+        图片名称，默认为None，不保存图片
+    show : bool
+        是否显示图片，默认为True
+    ax: matplotlib axes object
+        用于将图片绘制到matplotlib的子图上
+    **kwargs : dict
+        其他参数，如线条宽度、颜色等，传递给plt.plot函数
+
+    Returns
+    -------
+    MSD分析后的图片
+
+    Examples
+    --------
+    >>> from dspawpy.analysis.aimdtools import get_lagtime_msd, plot_msd
+
+    指定h5文件位置，用 get_lagtime_msd 函数获取数据，select 参数选择第n个原子（不是元素）
+
+    >>> lagtime, msd = get_lagtime_msd('/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', select=[0])
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    Calculating MSD...
+
+    用获取的数据画图并保存
+
+    >>> plot_msd(lagtime, msd, figname='/data/home/hzw1002/dspawpy_repo/test/out/MSD.png', show=False)
+    MSD图片保存在 /data/home/hzw1002/dspawpy_repo/test/out/MSD.png
+    <Axes: xlabel='Time (fs)', ylabel='MSD (Å)'>
+    """
+    if ax:
+        ishow = False
+        ax.plot(lagtime, result, c="black", ls="-", **kwargs)
+    else:
+        ishow = True
+        fig, ax = plt.subplots()
+        ax.plot(lagtime, result, c="black", ls="-", **kwargs)
+        ax.set_xlabel("Time (fs)")
+        ax.set_ylabel("MSD (Å)")
+
+    if xlim:
+        ax.set_xlim(xlim)
+    if ylim:
+        ax.set_ylim(ylim)
+
+    plt.tight_layout()
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print("MSD图片保存在", os.path.abspath(figname))
+    if show and ishow:  # 画子图的话，不应每个子图都show
+        plt.show()  # show会自动清空图片
+
+    return ax
+
+
+def plot_rdf(
+    rs: np.ndarray,
+    rdfs: np.ndarray,
+    ele1: str,
+    ele2: str,
+    xlim: list = None,
+    ylim: list = None,
+    figname: str = None,
+    show: bool = True,
+    ax: plt.Axes = None,
+    **kwargs,
+):
+    r"""AIMD计算后分析rdf并画图
+
+    Parameters
+    ----------
+    rs : numpy.ndarray
+        径向分布网格点
+    rdfs : numpy.ndarray
+        径向分布函数
+    ele1 : list
+        中心元素
+    ele2 : list
+        相邻元素
+    xlim : list
+        x轴范围，默认为None，即自动设置
+    ylim : list
+        y轴范围，默认为None，即自动设置
+    figname : str
+        图片名称，默认为None，即不保存图片
+    show : bool
+        是否显示图片，默认为True
+    ax: matplotlib.axes.Axes
+        画图的坐标轴，默认为None，即新建坐标轴
+    **kwargs : dict
+        其他参数，如线条宽度、颜色等，传递给plt.plot函数
+
+    Returns
+    -------
+    rdf分析后的图片
+
+    Examples
+    --------
+    >>> from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
+
+    先获取rs和rdfs数据作为xy轴数据
+
+    >>> rs, rdfs = get_rs_rdfs('/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', 'H', 'O', rmax=6)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    Calculating RDF...
+
+    将xy轴数据传入plot_rdf函数绘图
+
+    >>> plot_rdf(rs, rdfs, 'H','O', figname='/data/home/hzw1002/dspawpy_repo/test/out/RDF.png', show=False)
+    图片已保存到 /data/home/hzw1002/dspawpy_repo/test/out/RDF.png
+    """
+
+    if ax:
+        ishow = False
+        ax.plot(
+            rs,
+            rdfs,
+            label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
+            **kwargs,
+        )
+
+    else:
+        ishow = True
+        fig, ax = plt.subplots()
+        ax.plot(
+            rs,
+            rdfs,
+            label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
+            **kwargs,
+        )
+
+        ax.set_xlabel(r"$r$" + "(Å)")
+        ax.set_ylabel(r"$g(r)$")
+
+    ax.legend()
+
+    # 绘图细节
+    if xlim:
+        ax.set_xlim(xlim)
+    if ylim:
+        ax.set_ylim(ylim)
+
+    plt.tight_layout()
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"图片已保存到 {os.path.abspath(figname)}")
+    if show and ishow:  # 画子图的话，不应每个子图都show
+        plt.show()  # show会自动清空图片
+
+
+def plot_rmsd(
+    lagtime: np.ndarray,
+    result: np.ndarray,
+    xlim: list = None,
+    ylim: list = None,
+    figname: str = None,
+    show: bool = True,
+    ax=None,
+    **kwargs,
+):
+    r"""AIMD计算后分析rmsd并画图
+
+    Parameters
+    ----------
+    lagtime:
+        时间序列
+    result:
+        均方根序列
+    xlim : list
+        x轴范围
+    ylim : list
+        y轴范围
+    figname : str
+        图片保存路径
+    show : bool
+        是否显示图片
+    ax : matplotlib.axes._subplots.AxesSubplot
+        画子图的话，传入子图对象
+    **kwargs : dict
+        传入plt.plot的参数
+
+    Returns
+    -------
+    rmsd分析结构的图片
+
+    Examples
+    --------
+    >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
+
+    timestep 表示时间步长
+
+    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', timestep=0.1)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    Calculating RMSD...
+
+    直接保存为RMSD.png图片
+
+    >>> plot_rmsd(lagtime, rmsd, figname='/data/home/hzw1002/dspawpy_repo/test/out/RMSD.png', show=False)
+    图片已保存到 /data/home/hzw1002/dspawpy_repo/test/out/RMSD.png
+    <Axes: xlabel='Time (fs)', ylabel='RMSD (Å)'>
+    """
+    # 参数初始化
+    if not ax:
+        ishow = True
+    else:
+        ishow = False
+
+    if ax:
+        ax.plot(lagtime, result, **kwargs)
+    else:
+        fig, ax = plt.subplots()
+        ax.plot(lagtime, result, **kwargs)
+        ax.set_xlabel("Time (fs)")
+        ax.set_ylabel("RMSD (Å)")
+
+    if xlim:
+        ax.set_xlim(xlim)
+    if ylim:
+        ax.set_ylim(ylim)
+
+    plt.tight_layout()
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"图片已保存到 {os.path.abspath(figname)}")
+    if show and ishow:  # 画子图的话，不应每个子图都show
+        plt.show()  # show会自动清空图片
+
+    return ax
```

## dspawpy/analysis/vacf.py

 * *Ordering differences only*

```diff
@@ -1,555 +1,555 @@
-"""
-This module has not been tested yet, use at your own risk!
-"""
-
-import numpy as np
-from scipy.fftpack import fft
-from scipy.integrate import simps
-
-
-def welch(M, sym=1):
-    """Welch window. Function skeleton shamelessly stolen from
-    scipy.signal.bartlett() and others."""
-    if M < 1:
-        return np.array([])
-    if M == 1:
-        return np.ones(1, dtype=float)
-    odd = M % 2
-    if not sym and not odd:
-        M = M + 1
-    n = np.arange(0, M)
-    w = 1.0 - ((n - 0.5 * (M - 1)) / (0.5 * (M - 1))) ** 2.0
-    if not sym and not odd:
-        w = w[:-1]
-    return w
-
-
-def mirror(arr, axis=0):
-    """Mirror array `arr` at index 0 along `axis`.
-    The length of the returned array is 2*arr.shape[axis]-1 ."""
-    return np.concatenate((arr[::-1], arr[1:]), axis=axis)
-
-
-def pad_zeros(
-    arr, axis=0, where="end", nadd=None, upto=None, tonext=None, tonext_min=None
-):
-    """Pad an nd-array with zeros. Default is to append an array of zeros of
-    the same shape as `arr` to arr's end along `axis`.
-    Parameters
-    ----------
-    arr :  nd array
-    axis : the axis along which to pad
-    where : string {'end', 'start'}, pad at the end ("append to array") or
-        start ("prepend to array") of `axis`
-    nadd : number of items to padd (i.e. nadd=3 means padd w/ 3 zeros in case
-        of an 1d array)
-    upto : pad until arr.shape[axis] == upto
-    tonext : bool, pad up to the next power of two (pad so that the padded
-        array has a length of power of two)
-    tonext_min : int, when using `tonext`, pad the array to the next possible
-        power of two for which the resulting array length along `axis` is at
-        least `tonext_min`; the default is tonext_min = arr.shape[axis]
-    Use only one of nadd, upto, tonext.
-    Returns
-    -------
-    padded array
-    Examples
-    --------
-    >>> # 1d
-    >>> pad_zeros(a)
-    array([1, 2, 3, 0, 0, 0])
-    >>> pad_zeros(a, nadd=3)
-    array([1, 2, 3, 0, 0, 0])
-    >>> pad_zeros(a, upto=6)
-    array([1, 2, 3, 0, 0, 0])
-    >>> pad_zeros(a, nadd=1)
-    array([1, 2, 3, 0])
-    >>> pad_zeros(a, nadd=1, where='start')
-    array([0, 1, 2, 3])
-    >>> # 2d
-    >>> a=arange(9).reshape(3,3)
-    >>> pad_zeros(a, nadd=1, axis=0)
-    array([[0, 1, 2],
-           [3, 4, 5],
-           [6, 7, 8],
-           [0, 0, 0]])
-    >>> pad_zeros(a, nadd=1, axis=1)
-    array([[0, 1, 2, 0],
-           [3, 4, 5, 0],
-           [6, 7, 8, 0]])
-    >>> # up to next power of two
-    >>> 2**arange(10)
-    array([  1,   2,   4,   8,  16,  32,  64, 128, 256, 512])
-    >>> pydos.pad_zeros(arange(9), tonext=True).shape
-    (16,)
-    """
-    if tonext == False:
-        tonext = None
-    lst = [nadd, upto, tonext]
-    assert lst.count(None) in [2, 3], (
-        "`nadd`, `upto` and `tonext` must be " + "all None or only one of them not None"
-    )
-    if nadd is None:
-        if upto is None:
-            if (tonext is None) or (not tonext):
-                # default
-                nadd = arr.shape[axis]
-            else:
-                tonext_min = arr.shape[axis] if (tonext_min is None) else tonext_min
-                # beware of int overflows starting w/ 2**arange(64), but we
-                # will never have such long arrays anyway
-                two_powers = 2 ** np.arange(30)
-                assert tonext_min <= two_powers[-1], (
-                    "tonext_min exceeds " "max power of 2"
-                )
-                power = two_powers[np.searchsorted(two_powers, tonext_min)]
-                nadd = power - arr.shape[axis]
-        else:
-            nadd = upto - arr.shape[axis]
-    if nadd == 0:
-        return arr
-    add_shape = list(arr.shape)
-    add_shape[axis] = nadd
-    add_shape = tuple(add_shape)
-    if where == "end":
-        return np.concatenate((arr, np.zeros(add_shape, dtype=arr.dtype)), axis=axis)
-    elif where == "start":
-        return np.concatenate((np.zeros(add_shape, dtype=arr.dtype), arr), axis=axis)
-    else:
-        raise Exception("illegal `where` arg: %s" % where)
-
-
-def slicetake(a, sl, axis=None, copy=False):
-    """The equivalent of numpy.take(a, ..., axis=<axis>), but accepts slice
-    objects instead of an index array. Also by default, it returns a *view* and
-    no copy.
-    Parameters
-    ----------
-    a : numpy ndarray
-    sl : slice object, list or tuple of slice objects
-        axis=<int>
-            one slice object for *that* axis
-        axis=None
-            `sl` is a list or tuple of slice objects, one for each axis.
-            It must index the whole array, i.e. len(sl) == len(a.shape).
-    axis : {None, int}
-    copy : bool, return a copy instead of a view
-    Returns
-    -------
-    A view into `a` or copy of a slice of `a`.
-    Examples
-    --------
-    >>> from numpy import s_
-    >>> a = np.random.rand(20,20,20)
-    >>> b1 = a[:,:,10:]
-    >>> # single slice for axis 2
-    >>> b2 = slicetake(a, s_[10:], axis=2)
-    >>> # tuple of slice objects
-    >>> b3 = slicetake(a, s_[:,:,10:])
-    >>> (b2 == b1).all()
-    True
-    >>> (b3 == b1).all()
-    True
-    >>> # simple extraction too, sl = integer
-    >>> (a[...,5] == slicetake(a, 5, axis=-1))
-    True
-    """
-    # The long story
-    # --------------
-    #
-    # 1) Why do we need that:
-    #
-    # # no problem
-    # a[5:10:2]
-    #
-    # # the same, more general
-    # sl = slice(5,10,2)
-    # a[sl]
-    #
-    # But we want to:
-    #  - Define (type in) a slice object only once.
-    #  - Take the slice of different arrays along different axes.
-    # Since numpy.take() and a.take() don't handle slice objects, one would
-    # have to use direct slicing and pay attention to the shape of the array:
-    #
-    #     a[sl], b[:,:,sl,:], etc ...
-    #
-    # We want to use an 'axis' keyword instead. np.r_() generates index arrays
-    # from slice objects (e.g r_[1:5] == r_[s_[1:5] ==r_[slice(1,5,None)]).
-    # Since we need index arrays for numpy.take(), maybe we can use that? Like
-    # so:
-    #
-    #     a.take(r_[sl], axis=0)
-    #     b.take(r_[sl], axis=2)
-    #
-    # Here we have what we want: slice object + axis kwarg.
-    # But r_[slice(...)] does not work for all slice types. E.g. not for
-    #
-    #     r_[s_[::5]] == r_[slice(None, None, 5)] == array([], dtype=int32)
-    #     r_[::5]                                 == array([], dtype=int32)
-    #     r_[s_[1:]]  == r_[slice(1, None, None)] == array([0])
-    #     r_[1:]
-    #         ValueError: dimensions too large.
-    #
-    # The returned index arrays are wrong (or we even get an exception).
-    # The reason is given below.
-    # Bottom line: We need this function.
-    #
-    # The reason for r_[slice(...)] gererating sometimes wrong index arrays is
-    # that s_ translates a fancy index (1:, ::5, 1:10:2, ...) to a slice
-    # object. This *always* works. But since take() accepts only index arrays,
-    # we use r_[s_[<fancy_index>]], where r_ translates the slice object
-    # prodced by s_ to an index array. THAT works only if start and stop of the
-    # slice are known. r_ has no way of knowing the dimensions of the array to
-    # be sliced and so it can't transform a slice object into a correct index
-    # array in case of slice(<number>, None, None) or slice(None, None,
-    # <number>).
-    #
-    # 2) Slice vs. copy
-    #
-    # numpy.take(a, array([0,1,2,3])) or a[array([0,1,2,3])] return a copy of
-    # `a` b/c that's "fancy indexing". But a[slice(0,4,None)], which is the
-    # same as indexing (slicing) a[:4], return *views*.
-
-    if axis is None:
-        slices = sl
-    else:
-        # Note that these are equivalent:
-        #   a[:]
-        #   a[s_[:]]
-        #   a[slice(None)]
-        #   a[slice(None, None, None)]
-        #   a[slice(0, None, None)]
-        slices = [slice(None)] * a.ndim
-        slices[axis] = sl
-    # a[...] can take a tuple or list of slice objects
-    # a[x:y:z, i:j:k] is the same as
-    # a[(slice(x,y,z), slice(i,j,k))] == a[[slice(x,y,z), slice(i,j,k)]]
-    slices = tuple(slices)
-    if copy:
-        return a[slices].copy()
-    else:
-        return a[slices]
-
-
-def sum(arr, axis=None, keepdims=False, **kwds):
-    """This numpy.sum() with some features implemented which can be found in
-    numpy v1.7 and later: `axis` can be a tuple to select arbitrary axes to sum
-    over.
-    We also have a `keepdims` keyword, which however works completely different
-    from numpy. Docstrings shamelessly stolen from numpy and adapted here
-    and there.
-    Parameters
-    ----------
-    arr : nd array
-    axis : None or int or tuple of ints, optional
-        Axis or axes along which a sum is performed. The default (`axis` =
-        `None`) is to perform a sum over all the dimensions of the input array.
-        `axis` may be negative, in which case it counts from the last to the
-        first axis.
-        If this is a tuple of ints, a sum is performed on multiple
-        axes, instead of a single axis or all the axes as before.
-    keepdims : bool, optional
-        If this is set to True, the axes from `axis` are left in the result
-        and the reduction (sum) is performed for all remaining axes. Therefore,
-        it reverses the `axis` to be summed over.
-    **kwds : passed to np.sum().
-    Examples
-    --------
-    >>> a=rand(2,3,4)
-    >>> num.sum(a)
-    12.073636268676152
-    >>> a.sum()
-    12.073636268676152
-    >>> num.sum(a, axis=1).shape
-    (2, 4)
-    >>> num.sum(a, axis=(1,)).shape
-    (2, 4)
-    >>> # same as axis=1, i.e. it inverts the axis over which we sum
-    >>> num.sum(a, axis=(0,2), keepdims=True).shape
-    (2, 4)
-    >>> # numpy's keepdims has another meaning: it leave the summed axis (0,2)
-    >>> # as dimension of size 1 to allow broadcasting
-    >>> numpy.sum(a, axis=(0,2), keepdims=True).shape
-    (1, 3, 1)
-    >>> num.sum(a, axis=(1,)) - num.sum(a, axis=1)
-    array([[ 0.,  0.,  0.,  0.],
-           [ 0.,  0.,  0.,  0.]])
-    >>> num.sum(a, axis=(0,2)).shape
-    (3,)
-    >>> num.sum(a, axis=(0,2)) - a.sum(axis=0).sum(axis=1)
-    array([ 0.,  0.,  0.])
-    """
-
-    # Recursion rocks!
-    def _sum(arr, tosum):
-        if len(tosum) > 0:
-            # Choose axis to sum over, remove from list w/ remaining axes.
-            axis = tosum.pop(0)
-            _arr = arr.sum(axis=axis)
-            # arr has one dim less now. Rename remaining axes accordingly.
-            _tosum = [xx - 1 if xx > axis else xx for xx in tosum]
-            return _sum(_arr, _tosum)
-        else:
-            return arr
-
-    axis_is_int = isinstance(axis, int)
-    if axis is None:
-        if keepdims:
-            raise Exception("axis=None + keepdims=True makes no sense")
-        else:
-            return np.sum(arr, axis=axis, **kwds)
-    elif axis_is_int and not keepdims:
-        return np.sum(arr, axis=axis, **kwds)
-    else:
-        if axis_is_int:
-            tosum = [axis]
-        elif isinstance(axis, tuple) or isinstance(axis, list):
-            tosum = list(axis)
-        else:
-            raise Exception("illegal type for axis: %s" % str(type(axis)))
-        if keepdims:
-            alldims = range(arr.ndim)
-            tosum = [xx for xx in alldims if xx not in tosum]
-        return _sum(arr, tosum)
-
-
-def norm_int(y, x, area=1.0, scale=True, func=simps):
-    """Normalize integral area of y(x) to `area`.
-    Parameters
-    ----------
-    x,y : numpy 1d arrays
-    area : float
-    scale : bool, optional
-        Scale x and y to the same order of magnitude before integration.
-        This may be necessary to avoid numerical trouble if x and y have very
-        different scales.
-    func : callable
-        Function to do integration (like scipy.integrate.{simps,trapz,...}
-        Called as ``func(y,x)``. Default: simps
-    Returns
-    -------
-    scaled y
-    Notes
-    -----
-    The argument order y,x might be confusing. x,y would be more natural but we
-    stick to the order used in the scipy.integrate routines.
-    """
-    if scale:
-        fx = np.abs(x).max()
-        fy = np.abs(y).max()
-        sx = x / fx
-        sy = y / fy
-    else:
-        fx = fy = 1.0
-        sx, sy = x, y
-    # Area under unscaled y(x).
-    _area = func(sy, sx) * fx * fy
-    return y * area / _area
-
-
-def vacf(vel, m=None, method=3):
-    """Reference implementation for calculating the VACF of velocities in 3d
-    array `vel`. This is slow. Use for debugging only. For production, use
-    fvacf().
-
-    Parameters
-    ----------
-    vel : 3d array, (nstep, natoms, 3)
-        Atomic velocities.
-    m : 1d array (natoms,)
-        Atomic masses.
-    method : int
-        | 1 : 3 loops
-        | 2 : replace 1 inner loop
-        | 3 : replace 2 inner loops
-
-    Returns
-    -------
-    c : 1d array (nstep,)
-        VACF
-    """
-    natoms = vel.shape[1]
-    nstep = vel.shape[0]
-    c = np.zeros((nstep,), dtype=float)
-    if m is None:
-        m = np.ones((natoms,), dtype=float)
-    if method == 1:
-        # c(t) = <v(t0) v(t0 + t)> / <v(t0)**2> = C(t) / C(0)
-        #
-        # "displacements" `t'
-        for t in range(nstep):
-            # time origins t0 == j
-            for j in range(nstep - t):
-                for i in range(natoms):
-                    c[t] += np.dot(vel[j, i, :], vel[j + t, i, :]) * m[i]
-    elif method == 2:
-        # replace 1 inner loop
-        for t in range(nstep):
-            for j in range(nstep - t):
-                # (natoms, 3) * (natoms, 1) -> (natoms, 3)
-                c[t] += (vel[j, ...] * vel[j + t, ...] * m[:, None]).sum()
-    elif method == 3:
-        # replace 2 inner loops:
-        # (xx, natoms, 3) * (1, natoms, 1) -> (xx, natoms, 3)
-        for t in range(nstep):
-            c[t] = (vel[: (nstep - t), ...] * vel[t:, ...] * m[None, :, None]).sum()
-    else:
-        raise ValueError("unknown method: %s" % method)
-    # normalize to unity
-    c = c / c[0]
-    return c
-
-
-def pdos(
-    vel,
-    dt=1.0,
-    m=None,
-    full_out=False,
-    area=1.0,
-    window=True,
-    npad=None,
-    tonext=False,
-    mirr=False,
-    method="direct",
-):
-    """Phonon DOS by FFT of the VACF or direct FFT of atomic velocities.
-
-    Integral area is normalized to `area`. It is possible (and recommended) to
-    zero-padd the velocities (see `npad`).
-
-    Parameters
-    ----------
-    vel : 3d array (nstep, natoms, 3)
-        atomic velocities
-    dt : time step
-    m : 1d array (natoms,),
-        atomic mass array, if None then mass=1.0 for all atoms is used
-    full_out : bool
-    area : float
-        normalize area under frequency-PDOS curve to this value
-    window : bool
-        use Welch windowing on data before FFT (reduces leaking effect,
-        recommended)
-    npad : {None, int}
-        method='direct' only: Length of zero padding along `axis`. `npad=None`
-        = no padding, `npad > 0` = pad by a length of ``(nstep-1)*npad``. `npad
-        > 5` usually results in sufficient interpolation.
-    tonext : bool
-        method='direct' only: Pad `vel` with zeros along `axis` up to the next
-        power of two after the array length determined by `npad`. This gives
-        you speed, but variable (better) frequency resolution.
-    mirr : bool
-        method='vacf' only: mirror one-sided VACF at t=0 before fft
-
-    Returns
-    -------
-    if full_out = False
-        | ``(faxis, pdos)``
-        | faxis : 1d array [1/unit(dt)]
-        | pdos : 1d array, the phonon DOS, normalized to `area`
-    if full_out = True
-        | if method == 'direct':
-        |     ``(faxis, pdos, (full_faxis, full_pdos, split_idx))``
-        | if method == 'vavcf':
-        |     ``(faxis, pdos, (full_faxis, full_pdos, split_idx, vacf, fft_vacf))``
-        |     fft_vacf : 1d complex array, result of fft(vacf) or fft(mirror(vacf))
-        |     vacf : 1d array, the VACF
-
-    Notes
-    -----
-    padding (only method='direct'): With `npad` we pad the velocities `vel`
-    with ``npad*(nstep-1)`` zeros along `axis` (the time axis) before FFT
-    b/c the signal is not periodic. For `npad=1`, this gives us the exact
-    same spectrum and frequency resolution as with ``pdos(...,
-    method='vacf',mirr=True)`` b/c the array to be fft'ed has length
-    ``2*nstep-1`` along the time axis in both cases (remember that the
-    array length = length of the time axis influences the freq.
-    resolution). FFT is only fast for arrays with length = a power of two.
-    Therefore, you may get very different fft speeds depending on whether
-    ``2*nstep-1`` is a power of two or not (in most cases it won't). Try
-    using `tonext` but remember that you get another (better) frequency
-    resolution.
-
-    References
-    ----------
-    [1] Phys Rev B 47(9) 4863, 1993
-
-    See Also
-    --------
-    :func:`pwtools.signal.fftsample`
-    :func:`pwtools.signal.acorr`
-    :func:`direct_pdos`
-    :func:`vacf_pdos`
-
-    """
-    mass = m
-    # assume vel.shape = (nstep,natoms,3)
-    axis = 0
-    assert vel.shape[-1] == 3
-    if mass is not None:
-        assert len(mass) == vel.shape[1], "len(mass) != vel.shape[1]"
-        # define here b/c may be used twice below
-        mass_bc = mass[None, :, None]
-    if window:
-        sl = [None] * vel.ndim
-        sl[axis] = slice(None)  # ':'
-        vel2 = vel * (welch(vel.shape[axis])[tuple(sl)])
-    else:
-        vel2 = vel
-    # handle options which are mutually exclusive
-    if method == "vacf":
-        assert npad in [0, None], "use npad={0,None} for method='vacf'"
-    # padding
-    if npad is not None:
-        nadd = (vel2.shape[axis] - 1) * npad
-        if tonext:
-            vel2 = pad_zeros(
-                vel2, tonext=True, tonext_min=vel2.shape[axis] + nadd, axis=axis
-            )
-        else:
-            vel2 = pad_zeros(vel2, tonext=False, nadd=nadd, axis=axis)
-    if method == "direct":
-        full_fft_vel = np.abs(fft(vel2, axis=axis)) ** 2.0
-        full_faxis = np.fft.fftfreq(vel2.shape[axis], dt)
-        split_idx = len(full_faxis) // 2
-        faxis = full_faxis[:split_idx]
-        # First split the array, then multiply by `mass` and average. If
-        # full_out, then we need full_fft_vel below, so copy before slicing.
-        arr = full_fft_vel.copy() if full_out else full_fft_vel
-        # fft_vel = num.slicetake(arr, slice(0, split_idx), axis=axis, copy=False)
-        fft_vel = slicetake(arr, slice(0, split_idx), axis=axis, copy=False)
-        if mass is not None:
-            fft_vel *= mass_bc
-        # average remaining axes, summing is enough b/c normalization is done below
-        # sums: (nstep, natoms, 3) -> (nstep, natoms) -> (nstep,)
-        pdos = sum(fft_vel, axis=axis, keepdims=True)
-        default_out = (faxis, norm_int(pdos, faxis, area=area))
-        if full_out:
-            # have to re-calculate this here b/c we never calculate the full_pdos
-            # normally
-            if mass is not None:
-                full_fft_vel *= mass_bc
-            full_pdos = sum(full_fft_vel, axis=axis, keepdims=True)
-            extra_out = (full_faxis, full_pdos, split_idx)
-            return default_out + extra_out
-        else:
-            return default_out
-    elif method == "vacf":
-        # vacf = fvacf(vel2, m=mass)
-        vacf_ = vacf(vel2, m=mass)
-        if mirr:
-            fft_vacf = fft(mirror(vacf_))
-        else:
-            fft_vacf = fft(vacf_)
-        full_faxis = np.fft.fftfreq(fft_vacf.shape[axis], dt)
-        full_pdos = np.abs(fft_vacf)
-        split_idx = len(full_faxis) // 2
-        faxis = full_faxis[:split_idx]
-        pdos = full_pdos[:split_idx]
-        default_out = (faxis, norm_int(pdos, faxis, area=area))
-        extra_out = (full_faxis, full_pdos, split_idx, vacf_, fft_vacf)
-        if full_out:
-            return default_out + extra_out
-        else:
-            return default_out
+"""
+This module has not been tested yet, use at your own risk!
+"""
+
+import numpy as np
+from scipy.fftpack import fft
+from scipy.integrate import simps
+
+
+def welch(M, sym=1):
+    """Welch window. Function skeleton shamelessly stolen from
+    scipy.signal.bartlett() and others."""
+    if M < 1:
+        return np.array([])
+    if M == 1:
+        return np.ones(1, dtype=float)
+    odd = M % 2
+    if not sym and not odd:
+        M = M + 1
+    n = np.arange(0, M)
+    w = 1.0 - ((n - 0.5 * (M - 1)) / (0.5 * (M - 1))) ** 2.0
+    if not sym and not odd:
+        w = w[:-1]
+    return w
+
+
+def mirror(arr, axis=0):
+    """Mirror array `arr` at index 0 along `axis`.
+    The length of the returned array is 2*arr.shape[axis]-1 ."""
+    return np.concatenate((arr[::-1], arr[1:]), axis=axis)
+
+
+def pad_zeros(
+    arr, axis=0, where="end", nadd=None, upto=None, tonext=None, tonext_min=None
+):
+    """Pad an nd-array with zeros. Default is to append an array of zeros of
+    the same shape as `arr` to arr's end along `axis`.
+    Parameters
+    ----------
+    arr :  nd array
+    axis : the axis along which to pad
+    where : string {'end', 'start'}, pad at the end ("append to array") or
+        start ("prepend to array") of `axis`
+    nadd : number of items to padd (i.e. nadd=3 means padd w/ 3 zeros in case
+        of an 1d array)
+    upto : pad until arr.shape[axis] == upto
+    tonext : bool, pad up to the next power of two (pad so that the padded
+        array has a length of power of two)
+    tonext_min : int, when using `tonext`, pad the array to the next possible
+        power of two for which the resulting array length along `axis` is at
+        least `tonext_min`; the default is tonext_min = arr.shape[axis]
+    Use only one of nadd, upto, tonext.
+    Returns
+    -------
+    padded array
+    Examples
+    --------
+    >>> # 1d
+    >>> pad_zeros(a)
+    array([1, 2, 3, 0, 0, 0])
+    >>> pad_zeros(a, nadd=3)
+    array([1, 2, 3, 0, 0, 0])
+    >>> pad_zeros(a, upto=6)
+    array([1, 2, 3, 0, 0, 0])
+    >>> pad_zeros(a, nadd=1)
+    array([1, 2, 3, 0])
+    >>> pad_zeros(a, nadd=1, where='start')
+    array([0, 1, 2, 3])
+    >>> # 2d
+    >>> a=arange(9).reshape(3,3)
+    >>> pad_zeros(a, nadd=1, axis=0)
+    array([[0, 1, 2],
+           [3, 4, 5],
+           [6, 7, 8],
+           [0, 0, 0]])
+    >>> pad_zeros(a, nadd=1, axis=1)
+    array([[0, 1, 2, 0],
+           [3, 4, 5, 0],
+           [6, 7, 8, 0]])
+    >>> # up to next power of two
+    >>> 2**arange(10)
+    array([  1,   2,   4,   8,  16,  32,  64, 128, 256, 512])
+    >>> pydos.pad_zeros(arange(9), tonext=True).shape
+    (16,)
+    """
+    if tonext == False:
+        tonext = None
+    lst = [nadd, upto, tonext]
+    assert lst.count(None) in [2, 3], (
+        "`nadd`, `upto` and `tonext` must be " + "all None or only one of them not None"
+    )
+    if nadd is None:
+        if upto is None:
+            if (tonext is None) or (not tonext):
+                # default
+                nadd = arr.shape[axis]
+            else:
+                tonext_min = arr.shape[axis] if (tonext_min is None) else tonext_min
+                # beware of int overflows starting w/ 2**arange(64), but we
+                # will never have such long arrays anyway
+                two_powers = 2 ** np.arange(30)
+                assert tonext_min <= two_powers[-1], (
+                    "tonext_min exceeds " "max power of 2"
+                )
+                power = two_powers[np.searchsorted(two_powers, tonext_min)]
+                nadd = power - arr.shape[axis]
+        else:
+            nadd = upto - arr.shape[axis]
+    if nadd == 0:
+        return arr
+    add_shape = list(arr.shape)
+    add_shape[axis] = nadd
+    add_shape = tuple(add_shape)
+    if where == "end":
+        return np.concatenate((arr, np.zeros(add_shape, dtype=arr.dtype)), axis=axis)
+    elif where == "start":
+        return np.concatenate((np.zeros(add_shape, dtype=arr.dtype), arr), axis=axis)
+    else:
+        raise Exception("illegal `where` arg: %s" % where)
+
+
+def slicetake(a, sl, axis=None, copy=False):
+    """The equivalent of numpy.take(a, ..., axis=<axis>), but accepts slice
+    objects instead of an index array. Also by default, it returns a *view* and
+    no copy.
+    Parameters
+    ----------
+    a : numpy ndarray
+    sl : slice object, list or tuple of slice objects
+        axis=<int>
+            one slice object for *that* axis
+        axis=None
+            `sl` is a list or tuple of slice objects, one for each axis.
+            It must index the whole array, i.e. len(sl) == len(a.shape).
+    axis : {None, int}
+    copy : bool, return a copy instead of a view
+    Returns
+    -------
+    A view into `a` or copy of a slice of `a`.
+    Examples
+    --------
+    >>> from numpy import s_
+    >>> a = np.random.rand(20,20,20)
+    >>> b1 = a[:,:,10:]
+    >>> # single slice for axis 2
+    >>> b2 = slicetake(a, s_[10:], axis=2)
+    >>> # tuple of slice objects
+    >>> b3 = slicetake(a, s_[:,:,10:])
+    >>> (b2 == b1).all()
+    True
+    >>> (b3 == b1).all()
+    True
+    >>> # simple extraction too, sl = integer
+    >>> (a[...,5] == slicetake(a, 5, axis=-1))
+    True
+    """
+    # The long story
+    # --------------
+    #
+    # 1) Why do we need that:
+    #
+    # # no problem
+    # a[5:10:2]
+    #
+    # # the same, more general
+    # sl = slice(5,10,2)
+    # a[sl]
+    #
+    # But we want to:
+    #  - Define (type in) a slice object only once.
+    #  - Take the slice of different arrays along different axes.
+    # Since numpy.take() and a.take() don't handle slice objects, one would
+    # have to use direct slicing and pay attention to the shape of the array:
+    #
+    #     a[sl], b[:,:,sl,:], etc ...
+    #
+    # We want to use an 'axis' keyword instead. np.r_() generates index arrays
+    # from slice objects (e.g r_[1:5] == r_[s_[1:5] ==r_[slice(1,5,None)]).
+    # Since we need index arrays for numpy.take(), maybe we can use that? Like
+    # so:
+    #
+    #     a.take(r_[sl], axis=0)
+    #     b.take(r_[sl], axis=2)
+    #
+    # Here we have what we want: slice object + axis kwarg.
+    # But r_[slice(...)] does not work for all slice types. E.g. not for
+    #
+    #     r_[s_[::5]] == r_[slice(None, None, 5)] == array([], dtype=int32)
+    #     r_[::5]                                 == array([], dtype=int32)
+    #     r_[s_[1:]]  == r_[slice(1, None, None)] == array([0])
+    #     r_[1:]
+    #         ValueError: dimensions too large.
+    #
+    # The returned index arrays are wrong (or we even get an exception).
+    # The reason is given below.
+    # Bottom line: We need this function.
+    #
+    # The reason for r_[slice(...)] gererating sometimes wrong index arrays is
+    # that s_ translates a fancy index (1:, ::5, 1:10:2, ...) to a slice
+    # object. This *always* works. But since take() accepts only index arrays,
+    # we use r_[s_[<fancy_index>]], where r_ translates the slice object
+    # prodced by s_ to an index array. THAT works only if start and stop of the
+    # slice are known. r_ has no way of knowing the dimensions of the array to
+    # be sliced and so it can't transform a slice object into a correct index
+    # array in case of slice(<number>, None, None) or slice(None, None,
+    # <number>).
+    #
+    # 2) Slice vs. copy
+    #
+    # numpy.take(a, array([0,1,2,3])) or a[array([0,1,2,3])] return a copy of
+    # `a` b/c that's "fancy indexing". But a[slice(0,4,None)], which is the
+    # same as indexing (slicing) a[:4], return *views*.
+
+    if axis is None:
+        slices = sl
+    else:
+        # Note that these are equivalent:
+        #   a[:]
+        #   a[s_[:]]
+        #   a[slice(None)]
+        #   a[slice(None, None, None)]
+        #   a[slice(0, None, None)]
+        slices = [slice(None)] * a.ndim
+        slices[axis] = sl
+    # a[...] can take a tuple or list of slice objects
+    # a[x:y:z, i:j:k] is the same as
+    # a[(slice(x,y,z), slice(i,j,k))] == a[[slice(x,y,z), slice(i,j,k)]]
+    slices = tuple(slices)
+    if copy:
+        return a[slices].copy()
+    else:
+        return a[slices]
+
+
+def sum(arr, axis=None, keepdims=False, **kwds):
+    """This numpy.sum() with some features implemented which can be found in
+    numpy v1.7 and later: `axis` can be a tuple to select arbitrary axes to sum
+    over.
+    We also have a `keepdims` keyword, which however works completely different
+    from numpy. Docstrings shamelessly stolen from numpy and adapted here
+    and there.
+    Parameters
+    ----------
+    arr : nd array
+    axis : None or int or tuple of ints, optional
+        Axis or axes along which a sum is performed. The default (`axis` =
+        `None`) is to perform a sum over all the dimensions of the input array.
+        `axis` may be negative, in which case it counts from the last to the
+        first axis.
+        If this is a tuple of ints, a sum is performed on multiple
+        axes, instead of a single axis or all the axes as before.
+    keepdims : bool, optional
+        If this is set to True, the axes from `axis` are left in the result
+        and the reduction (sum) is performed for all remaining axes. Therefore,
+        it reverses the `axis` to be summed over.
+    **kwds : passed to np.sum().
+    Examples
+    --------
+    >>> a=rand(2,3,4)
+    >>> num.sum(a)
+    12.073636268676152
+    >>> a.sum()
+    12.073636268676152
+    >>> num.sum(a, axis=1).shape
+    (2, 4)
+    >>> num.sum(a, axis=(1,)).shape
+    (2, 4)
+    >>> # same as axis=1, i.e. it inverts the axis over which we sum
+    >>> num.sum(a, axis=(0,2), keepdims=True).shape
+    (2, 4)
+    >>> # numpy's keepdims has another meaning: it leave the summed axis (0,2)
+    >>> # as dimension of size 1 to allow broadcasting
+    >>> numpy.sum(a, axis=(0,2), keepdims=True).shape
+    (1, 3, 1)
+    >>> num.sum(a, axis=(1,)) - num.sum(a, axis=1)
+    array([[ 0.,  0.,  0.,  0.],
+           [ 0.,  0.,  0.,  0.]])
+    >>> num.sum(a, axis=(0,2)).shape
+    (3,)
+    >>> num.sum(a, axis=(0,2)) - a.sum(axis=0).sum(axis=1)
+    array([ 0.,  0.,  0.])
+    """
+
+    # Recursion rocks!
+    def _sum(arr, tosum):
+        if len(tosum) > 0:
+            # Choose axis to sum over, remove from list w/ remaining axes.
+            axis = tosum.pop(0)
+            _arr = arr.sum(axis=axis)
+            # arr has one dim less now. Rename remaining axes accordingly.
+            _tosum = [xx - 1 if xx > axis else xx for xx in tosum]
+            return _sum(_arr, _tosum)
+        else:
+            return arr
+
+    axis_is_int = isinstance(axis, int)
+    if axis is None:
+        if keepdims:
+            raise Exception("axis=None + keepdims=True makes no sense")
+        else:
+            return np.sum(arr, axis=axis, **kwds)
+    elif axis_is_int and not keepdims:
+        return np.sum(arr, axis=axis, **kwds)
+    else:
+        if axis_is_int:
+            tosum = [axis]
+        elif isinstance(axis, tuple) or isinstance(axis, list):
+            tosum = list(axis)
+        else:
+            raise Exception("illegal type for axis: %s" % str(type(axis)))
+        if keepdims:
+            alldims = range(arr.ndim)
+            tosum = [xx for xx in alldims if xx not in tosum]
+        return _sum(arr, tosum)
+
+
+def norm_int(y, x, area=1.0, scale=True, func=simps):
+    """Normalize integral area of y(x) to `area`.
+    Parameters
+    ----------
+    x,y : numpy 1d arrays
+    area : float
+    scale : bool, optional
+        Scale x and y to the same order of magnitude before integration.
+        This may be necessary to avoid numerical trouble if x and y have very
+        different scales.
+    func : callable
+        Function to do integration (like scipy.integrate.{simps,trapz,...}
+        Called as ``func(y,x)``. Default: simps
+    Returns
+    -------
+    scaled y
+    Notes
+    -----
+    The argument order y,x might be confusing. x,y would be more natural but we
+    stick to the order used in the scipy.integrate routines.
+    """
+    if scale:
+        fx = np.abs(x).max()
+        fy = np.abs(y).max()
+        sx = x / fx
+        sy = y / fy
+    else:
+        fx = fy = 1.0
+        sx, sy = x, y
+    # Area under unscaled y(x).
+    _area = func(sy, sx) * fx * fy
+    return y * area / _area
+
+
+def vacf(vel, m=None, method=3):
+    """Reference implementation for calculating the VACF of velocities in 3d
+    array `vel`. This is slow. Use for debugging only. For production, use
+    fvacf().
+
+    Parameters
+    ----------
+    vel : 3d array, (nstep, natoms, 3)
+        Atomic velocities.
+    m : 1d array (natoms,)
+        Atomic masses.
+    method : int
+        | 1 : 3 loops
+        | 2 : replace 1 inner loop
+        | 3 : replace 2 inner loops
+
+    Returns
+    -------
+    c : 1d array (nstep,)
+        VACF
+    """
+    natoms = vel.shape[1]
+    nstep = vel.shape[0]
+    c = np.zeros((nstep,), dtype=float)
+    if m is None:
+        m = np.ones((natoms,), dtype=float)
+    if method == 1:
+        # c(t) = <v(t0) v(t0 + t)> / <v(t0)**2> = C(t) / C(0)
+        #
+        # "displacements" `t'
+        for t in range(nstep):
+            # time origins t0 == j
+            for j in range(nstep - t):
+                for i in range(natoms):
+                    c[t] += np.dot(vel[j, i, :], vel[j + t, i, :]) * m[i]
+    elif method == 2:
+        # replace 1 inner loop
+        for t in range(nstep):
+            for j in range(nstep - t):
+                # (natoms, 3) * (natoms, 1) -> (natoms, 3)
+                c[t] += (vel[j, ...] * vel[j + t, ...] * m[:, None]).sum()
+    elif method == 3:
+        # replace 2 inner loops:
+        # (xx, natoms, 3) * (1, natoms, 1) -> (xx, natoms, 3)
+        for t in range(nstep):
+            c[t] = (vel[: (nstep - t), ...] * vel[t:, ...] * m[None, :, None]).sum()
+    else:
+        raise ValueError("unknown method: %s" % method)
+    # normalize to unity
+    c = c / c[0]
+    return c
+
+
+def pdos(
+    vel,
+    dt=1.0,
+    m=None,
+    full_out=False,
+    area=1.0,
+    window=True,
+    npad=None,
+    tonext=False,
+    mirr=False,
+    method="direct",
+):
+    """Phonon DOS by FFT of the VACF or direct FFT of atomic velocities.
+
+    Integral area is normalized to `area`. It is possible (and recommended) to
+    zero-padd the velocities (see `npad`).
+
+    Parameters
+    ----------
+    vel : 3d array (nstep, natoms, 3)
+        atomic velocities
+    dt : time step
+    m : 1d array (natoms,),
+        atomic mass array, if None then mass=1.0 for all atoms is used
+    full_out : bool
+    area : float
+        normalize area under frequency-PDOS curve to this value
+    window : bool
+        use Welch windowing on data before FFT (reduces leaking effect,
+        recommended)
+    npad : {None, int}
+        method='direct' only: Length of zero padding along `axis`. `npad=None`
+        = no padding, `npad > 0` = pad by a length of ``(nstep-1)*npad``. `npad
+        > 5` usually results in sufficient interpolation.
+    tonext : bool
+        method='direct' only: Pad `vel` with zeros along `axis` up to the next
+        power of two after the array length determined by `npad`. This gives
+        you speed, but variable (better) frequency resolution.
+    mirr : bool
+        method='vacf' only: mirror one-sided VACF at t=0 before fft
+
+    Returns
+    -------
+    if full_out = False
+        | ``(faxis, pdos)``
+        | faxis : 1d array [1/unit(dt)]
+        | pdos : 1d array, the phonon DOS, normalized to `area`
+    if full_out = True
+        | if method == 'direct':
+        |     ``(faxis, pdos, (full_faxis, full_pdos, split_idx))``
+        | if method == 'vavcf':
+        |     ``(faxis, pdos, (full_faxis, full_pdos, split_idx, vacf, fft_vacf))``
+        |     fft_vacf : 1d complex array, result of fft(vacf) or fft(mirror(vacf))
+        |     vacf : 1d array, the VACF
+
+    Notes
+    -----
+    padding (only method='direct'): With `npad` we pad the velocities `vel`
+    with ``npad*(nstep-1)`` zeros along `axis` (the time axis) before FFT
+    b/c the signal is not periodic. For `npad=1`, this gives us the exact
+    same spectrum and frequency resolution as with ``pdos(...,
+    method='vacf',mirr=True)`` b/c the array to be fft'ed has length
+    ``2*nstep-1`` along the time axis in both cases (remember that the
+    array length = length of the time axis influences the freq.
+    resolution). FFT is only fast for arrays with length = a power of two.
+    Therefore, you may get very different fft speeds depending on whether
+    ``2*nstep-1`` is a power of two or not (in most cases it won't). Try
+    using `tonext` but remember that you get another (better) frequency
+    resolution.
+
+    References
+    ----------
+    [1] Phys Rev B 47(9) 4863, 1993
+
+    See Also
+    --------
+    :func:`pwtools.signal.fftsample`
+    :func:`pwtools.signal.acorr`
+    :func:`direct_pdos`
+    :func:`vacf_pdos`
+
+    """
+    mass = m
+    # assume vel.shape = (nstep,natoms,3)
+    axis = 0
+    assert vel.shape[-1] == 3
+    if mass is not None:
+        assert len(mass) == vel.shape[1], "len(mass) != vel.shape[1]"
+        # define here b/c may be used twice below
+        mass_bc = mass[None, :, None]
+    if window:
+        sl = [None] * vel.ndim
+        sl[axis] = slice(None)  # ':'
+        vel2 = vel * (welch(vel.shape[axis])[tuple(sl)])
+    else:
+        vel2 = vel
+    # handle options which are mutually exclusive
+    if method == "vacf":
+        assert npad in [0, None], "use npad={0,None} for method='vacf'"
+    # padding
+    if npad is not None:
+        nadd = (vel2.shape[axis] - 1) * npad
+        if tonext:
+            vel2 = pad_zeros(
+                vel2, tonext=True, tonext_min=vel2.shape[axis] + nadd, axis=axis
+            )
+        else:
+            vel2 = pad_zeros(vel2, tonext=False, nadd=nadd, axis=axis)
+    if method == "direct":
+        full_fft_vel = np.abs(fft(vel2, axis=axis)) ** 2.0
+        full_faxis = np.fft.fftfreq(vel2.shape[axis], dt)
+        split_idx = len(full_faxis) // 2
+        faxis = full_faxis[:split_idx]
+        # First split the array, then multiply by `mass` and average. If
+        # full_out, then we need full_fft_vel below, so copy before slicing.
+        arr = full_fft_vel.copy() if full_out else full_fft_vel
+        # fft_vel = num.slicetake(arr, slice(0, split_idx), axis=axis, copy=False)
+        fft_vel = slicetake(arr, slice(0, split_idx), axis=axis, copy=False)
+        if mass is not None:
+            fft_vel *= mass_bc
+        # average remaining axes, summing is enough b/c normalization is done below
+        # sums: (nstep, natoms, 3) -> (nstep, natoms) -> (nstep,)
+        pdos = sum(fft_vel, axis=axis, keepdims=True)
+        default_out = (faxis, norm_int(pdos, faxis, area=area))
+        if full_out:
+            # have to re-calculate this here b/c we never calculate the full_pdos
+            # normally
+            if mass is not None:
+                full_fft_vel *= mass_bc
+            full_pdos = sum(full_fft_vel, axis=axis, keepdims=True)
+            extra_out = (full_faxis, full_pdos, split_idx)
+            return default_out + extra_out
+        else:
+            return default_out
+    elif method == "vacf":
+        # vacf = fvacf(vel2, m=mass)
+        vacf_ = vacf(vel2, m=mass)
+        if mirr:
+            fft_vacf = fft(mirror(vacf_))
+        else:
+            fft_vacf = fft(vacf_)
+        full_faxis = np.fft.fftfreq(fft_vacf.shape[axis], dt)
+        full_pdos = np.abs(fft_vacf)
+        split_idx = len(full_faxis) // 2
+        faxis = full_faxis[:split_idx]
+        pdos = full_pdos[:split_idx]
+        default_out = (faxis, norm_int(pdos, faxis, area=area))
+        extra_out = (full_faxis, full_pdos, split_idx, vacf_, fft_vacf)
+        if full_out:
+            return default_out + extra_out
+        else:
+            return default_out
```

## dspawpy/diffusion/neb.py

 * *Ordering differences only*

```diff
@@ -1,115 +1,115 @@
-import os
-
-from dspawpy.diffusion.pathfinder import IDPPSolver
-from dspawpy.io.write import to_file
-
-
-class NEB:
-    """NEB插值算法
-
-    Parameters
-    ----------
-    initial_structure: Structure
-        初态
-    final_structure: Structure
-        终态
-    nimages: int
-        中间构型数
-    """
-
-    def __init__(self, initial_structure, final_structure, nimages):
-        """
-
-        Args:
-            initial_structure:
-            final_structure:
-            nimages: number of images,contain initial and final structure
-        """
-
-        self.nimages = nimages
-        self.iddp = IDPPSolver.from_endpoints(
-            endpoints=[initial_structure, final_structure],
-            nimages=self.nimages - 2,
-            sort_tol=0,  # 锁定原子编号
-        )
-
-    def linear_interpolate(self):
-        return self.iddp.structures
-
-    def idpp_interpolate(
-        self,
-        maxiter=1000,
-        tol=1e-5,
-        gtol=1e-3,
-        step_size=0.05,
-        max_disp=0.05,
-        spring_const=5.0,
-    ):
-        return self.iddp.run(maxiter, tol, gtol, step_size, max_disp, spring_const)
-
-
-def write_neb_structures(
-    structures,
-    coords_are_cartesian=True,
-    fmt: str = "as",
-    path: str = ".",
-    prefix="structure",
-):
-    r"""插值并生成中间构型文件
-
-    Parameters
-    ----------
-    structures: list
-        构型列表
-    coords_are_cartesian: bool
-        坐标是否为笛卡尔坐标
-    fmt: str
-        结构文件类型，默认为 "as"
-    path: str
-        保存路径
-    prefix: str
-        文件名前缀，默认为 "structure"，这样的话生成的就是 structure00.as, structure01.as, ...
-
-    Returns
-    -------
-    file
-        保存构型文件
-
-    Examples
-    --------
-
-    先读取as文件创建structure对象
-
-    >>> from dspawpy.io.structure import build_Structures_from_datafile
-    >>> from dspawpy.diffusion.nebtools import write_movie_json
-
-    >>> init_struct = build_Structures_from_datafile("/data/home/hzw1002/dspawpy_repo/test/2.15/00/structure00.as")[0]
-    >>> final_struct = build_Structures_from_datafile("/data/home/hzw1002/dspawpy_repo/test/2.15/04/structure04.as")[0]
-
-    然后，插值并生成中间构型文件
-
-    >>> from dspawpy.diffusion.neb import NEB,write_neb_structures
-    >>> neb = NEB(init_struct,final_struct,8)
-    >>> structures = neb.linear_interpolate()   #线性插值
-
-    插值完成的构型可指定保存到neb文件夹下
-
-    >>> write_neb_structures(structures, fmt="as", path="/data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures")
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/00/structure00.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/01/structure01.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/02/structure02.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/03/structure03.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/04/structure04.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/05/structure05.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/06/structure06.as
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/07/structure07.as
-    """
-    assert fmt is not None
-    N = len(str(len(structures)))
-    if N <= 2:
-        N = 2
-    for i, structure in enumerate(structures):
-        path_name = str(i).zfill(N)
-        os.makedirs(os.path.join(path, path_name), exist_ok=True)
-        filename = os.path.join(path, path_name, "%s%s.%s" % (prefix, path_name, fmt))
-        to_file(structure, filename, fmt, coords_are_cartesian)
+import os
+
+from dspawpy.diffusion.pathfinder import IDPPSolver
+from dspawpy.io.write import to_file
+
+
+class NEB:
+    """NEB插值算法
+
+    Parameters
+    ----------
+    initial_structure: Structure
+        初态
+    final_structure: Structure
+        终态
+    nimages: int
+        中间构型数
+    """
+
+    def __init__(self, initial_structure, final_structure, nimages):
+        """
+
+        Args:
+            initial_structure:
+            final_structure:
+            nimages: number of images,contain initial and final structure
+        """
+
+        self.nimages = nimages
+        self.iddp = IDPPSolver.from_endpoints(
+            endpoints=[initial_structure, final_structure],
+            nimages=self.nimages - 2,
+            sort_tol=0,  # 锁定原子编号
+        )
+
+    def linear_interpolate(self):
+        return self.iddp.structures
+
+    def idpp_interpolate(
+        self,
+        maxiter=1000,
+        tol=1e-5,
+        gtol=1e-3,
+        step_size=0.05,
+        max_disp=0.05,
+        spring_const=5.0,
+    ):
+        return self.iddp.run(maxiter, tol, gtol, step_size, max_disp, spring_const)
+
+
+def write_neb_structures(
+    structures,
+    coords_are_cartesian=True,
+    fmt: str = "as",
+    path: str = ".",
+    prefix="structure",
+):
+    r"""插值并生成中间构型文件
+
+    Parameters
+    ----------
+    structures: list
+        构型列表
+    coords_are_cartesian: bool
+        坐标是否为笛卡尔坐标
+    fmt: str
+        结构文件类型，默认为 "as"
+    path: str
+        保存路径
+    prefix: str
+        文件名前缀，默认为 "structure"，这样的话生成的就是 structure00.as, structure01.as, ...
+
+    Returns
+    -------
+    file
+        保存构型文件
+
+    Examples
+    --------
+
+    先读取as文件创建structure对象
+
+    >>> from dspawpy.io.structure import build_Structures_from_datafile
+    >>> from dspawpy.diffusion.nebtools import write_movie_json
+
+    >>> init_struct = build_Structures_from_datafile("/data/home/hzw1002/dspawpy_repo/test/2.15/00/structure00.as")[0]
+    >>> final_struct = build_Structures_from_datafile("/data/home/hzw1002/dspawpy_repo/test/2.15/04/structure04.as")[0]
+
+    然后，插值并生成中间构型文件
+
+    >>> from dspawpy.diffusion.neb import NEB,write_neb_structures
+    >>> neb = NEB(init_struct,final_struct,8)
+    >>> structures = neb.linear_interpolate()   #线性插值
+
+    插值完成的构型可指定保存到neb文件夹下
+
+    >>> write_neb_structures(structures, fmt="as", path="/data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures")
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/00/structure00.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/01/structure01.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/02/structure02.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/03/structure03.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/04/structure04.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/05/structure05.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/06/structure06.as
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/11neb_interpolate_structures/07/structure07.as
+    """
+    assert fmt is not None
+    N = len(str(len(structures)))
+    if N <= 2:
+        N = 2
+    for i, structure in enumerate(structures):
+        path_name = str(i).zfill(N)
+        os.makedirs(os.path.join(path, path_name), exist_ok=True)
+        filename = os.path.join(path, path_name, "%s%s.%s" % (prefix, path_name, fmt))
+        to_file(structure, filename, fmt, coords_are_cartesian)
```

## dspawpy/diffusion/nebtools.py

```diff
@@ -1,1498 +1,1498 @@
-import json
-import os
-import shutil
-
-import h5py
-import numpy as np
-import pandas as pd
-
-np.set_printoptions(suppress=True)  # 不使用科学计数法
-import zipfile
-
-import matplotlib.pyplot as plt
-
-from dspawpy.io.structure import build_Structures_from_datafile
-from dspawpy.io.utils import get_ele_from_h5
-
-
-def _zip_folder(folder_path, output_path):
-    with zipfile.ZipFile(output_path, "w", zipfile.ZIP_DEFLATED) as zipf:
-        for root, _, files in os.walk(folder_path):
-            for file in files:
-                file_path = os.path.join(root, file)
-                zipf.write(file_path, os.path.relpath(file_path, folder_path))
-    print(f"已将{folder_path}压缩到{output_path}")
-
-
-def get_distance(
-    spo1: np.ndarray, spo2: np.ndarray, lat1: np.ndarray, lat2: np.ndarray
-):
-    r"""根据两个结构的分数坐标和晶胞计算距离
-
-    Parameters
-    ----------
-    spo1 : np.ndarray
-        分数坐标列表1
-    spo2 : np.ndarray
-        分数坐标列表2
-    lat1 : np.ndarray
-        晶胞1
-    lat2 : np.ndarray
-        晶胞2
-
-    Returns
-    -------
-    float
-        距离
-
-    Examples
-    --------
-
-    先读取结构信息
-
-    >>> from dspawpy.io.structure import build_Structures_from_datafile
-    >>> s1 = build_Structures_from_datafile('/data/home/hzw1002/dspawpy_repo/test/2.15/01/structure01.as')[0]
-    >>> s2 = build_Structures_from_datafile('/data/home/hzw1002/dspawpy_repo/test/2.15/02/structure02.as')[0]
-
-    计算两个构型的距离
-
-    >>> from dspawpy.diffusion.nebtools import get_distance
-    >>> dist = get_distance(s1.frac_coords, s2.frac_coords, s1.lattice.matrix, s2.lattice.matrix)
-    >>> print('两个构型的距离为：', dist, 'Angstrom')
-    两个构型的距离为： 0.476972808803491 Angstrom
-    """
-    diff_spo = spo1 - spo2  # 分数坐标差
-    avglatv = 0.5 * (lat1 + lat2)  # 平均晶格矢量
-    pbc_diff_spo = set_pbc(diff_spo)  # 笛卡尔坐标差
-    # 分数坐标点乘平均晶胞，转回笛卡尔坐标
-    pbc_diff_pos = np.dot(pbc_diff_spo, avglatv)  # 笛卡尔坐标差
-    distance = np.sqrt(np.sum(pbc_diff_pos**2))
-
-    return distance
-
-
-def get_neb_subfolders(directory: str = ".", return_abs=False):
-    r"""将directory路径下的子文件夹名称列表按照数字大小排序
-
-    仅保留形如00，01数字类型的NEB子文件夹路径
-
-    Parameters
-    ----------
-    subfolders : list
-        子文件夹名称列表
-    return_abs : bool, optional
-        是否返回绝对路径, 默认否
-
-    Returns
-    -------
-    subfolders : list
-        排序后的子文件夹名称列表
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.nebtools import get_neb_subfolders
-    >>> directory = '/data/home/hzw1002/dspawpy_repo/test/2.15'
-    >>> get_neb_subfolders(directory)
-    ['00', '01', '02', '03', '04']
-    """
-    raw_subfolders = next(os.walk(directory))[1]
-    subfolders = []
-    for subfolder in raw_subfolders:
-        try:
-            assert 0 <= int(subfolder) < 100
-            subfolders.append(subfolder)
-        except:
-            pass
-    subfolders.sort()  # 从小到大排序
-    if return_abs:
-        subfolders = [
-            os.path.abspath(os.path.join(directory, subfolder))
-            for subfolder in subfolders
-        ]
-    return subfolders
-
-
-def plot_barrier(
-    datafile: str = "neb.h5",
-    directory: str = None,
-    ri: float = None,
-    rf: float = None,
-    ei: float = None,
-    ef: float = None,
-    method: str = "PchipInterpolator",
-    figname: str = "neb_barrier.png",
-    show: bool = True,
-    raw=False,
-    **kwargs,
-):
-    r"""调用 scipy.interpolate 插值算法，拟合NEB能垒并绘图
-
-    Parameters
-    ----------
-    datafile: str
-        neb.h5或neb.json文件路径
-    directory : str
-        NEB计算路径
-    ri : float
-        初态反应坐标
-    rf : float
-        末态反应坐标
-    ei : float
-        初态自洽能量
-    ef : float
-        末态自洽能量
-    method : str, optional
-        插值算法, by default 'PchipInterpolator'
-    figname : str, optional
-        能垒图名称, by default 'neb_barrier.png'
-    show : bool, optional
-        是否展示交互界面, by default True
-    raw : bool, optional
-        是否返回原始数据到csv
-
-    Raises
-    ------
-    ImportError
-        指定了scipy.interpolate中不存在的插值算法
-    ValueError
-        传递给插值算法的参数不符合该算法要求
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.nebtools import plot_barrier
-    >>> import matplotlib.pyplot as plt
-    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='interp1d', kind=2, figname=None, show=False)
-    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='interp1d', kind=3, figname=None, show=False)
-    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='CubicSpline', figname=None, show=False)
-    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='pchip', figname=None, show=False)
-    """
-    if directory is not None:
-        # read data
-        subfolders, resort_mfs, rcs, ens, dEs = _getef(directory)
-
-    elif datafile:
-        assert os.path.exists(datafile), f"文件{datafile}不存在"
-        if datafile.endswith(".h5"):
-            from dspawpy.io.read import load_h5
-
-            neb = load_h5(datafile)
-            if "/BarrierInfo/ReactionCoordinate" in neb.keys():
-                reaction_coordinate = neb["/BarrierInfo/ReactionCoordinate"]
-                energy = neb["/BarrierInfo/TotalEnergy"]
-            else:  # old version
-                reaction_coordinate = neb["/Distance/ReactionCoordinate"]
-                energy = neb["/Energy/TotalEnergy"]
-        elif datafile.endswith(".json"):
-            with open(datafile, "r") as fin:
-                neb = json.load(fin)
-            if "BarrierInfo" in neb.keys():
-                reaction_coordinate = neb["BarrierInfo"]["ReactionCoordinate"]
-                energy = neb["BarrierInfo"]["TotalEnergy"]
-            else:  # old version
-                reaction_coordinate = neb["Distance"]["ReactionCoordinate"]
-                energy = neb["Energy"]["TotalEnergy"]
-        else:
-            raise TypeError("datafile 必须是 .h5 或 .json 文件格式")
-
-        x = []
-        for c in reaction_coordinate:
-            if len(x) > 0:
-                x.append(x[-1] + c)
-            else:
-                x.append(c)
-
-        y = [x - energy[0] for x in energy]
-        # initial and final info
-        if ri is not None:  # add initial reaction coordinate
-            x.insert(0, ri)
-        if rf is not None:  # add final reaction coordinate
-            x.append(rf)
-
-        if ei is not None:  # add initial energy
-            y.insert(0, ei)
-        if ef is not None:  # add final energy
-            y.append(ef)
-
-        rcs = np.array(x)
-        dEs = np.array(y)
-
-        print(f"如果NEB任务不计算初末态的自洽，{datafile}中将缺失相关信息，需要手动输入")
-        os.getcwd()
-
-    else:
-        raise ValueError("请指定datafile或directory！")
-
-    # import scipy interpolater
-    try:
-        interpolate_method = getattr(
-            __import__("scipy.interpolate", fromlist=[method]), method
-        )
-    except:
-        raise ImportError(f"无法找到 scipy.interpolate.{method} 算法！")
-    # call the interpolater to interpolate with given kwargs
-    try:
-        inter_f = interpolate_method(rcs, dEs, **kwargs)
-    except:
-        raise ValueError(f"插值失败，请检查{kwargs}参数设置是否有误！")
-
-    xnew = np.linspace(rcs[0], rcs[-1], 100)
-    ynew = inter_f(xnew)
-
-    if raw:
-        pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv", index=False)
-        pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
-            "raw_interpolated_xy.csv", index=False
-        )
-
-    # plot
-    if kwargs:
-        plt.plot(xnew, ynew, label=method + str(kwargs))
-    else:
-        plt.plot(xnew, ynew, label=method)
-    plt.scatter(rcs, dEs, c="r")
-    plt.xlabel("Reaction Coordinate (Å)")
-    plt.ylabel("Energy (eV)")
-    plt.legend()
-
-    plt.tight_layout()
-    # save and show
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
-    if show:
-        plt.show()
-
-
-def plot_neb_converge(
-    neb_dir: str,
-    image_key: str = "01",
-    show: bool = True,
-    figname: str = "neb_conv.png",
-    raw=False,
-):
-    """指定NEB计算路径，绘制NEB收敛过程图
-
-    Parameters
-    ----------
-    neb_dir : str
-        NEB计算路径
-    image_key : str
-        第几个构型，默认 "01"
-    show : bool
-        是否交互绘图
-    image_name : str
-        NEB收敛图名称，默认 "neb_conv.png"
-    raw : bool
-        是否输出原始数据到csv文件
-
-    Returns
-    -------
-    ax1, ax2 : matplotlib.axes.Axes
-        两个子图的Axes对象
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.nebtools import plot_neb_converge
-    >>> plot_neb_converge(neb_dir='/data/home/hzw1002/dspawpy_repo/test/2.15', image_key='01', figname='/data/home/hzw1002/dspawpy_repo/test/out/neb_converge1.png',show=False)
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/out/neb_converge1.png
-    (<Axes: xlabel='Number of ionic step', ylabel='Force (eV/Å)'>, <Axes: xlabel='Number of ionic step', ylabel='Energy (eV)'>)
-    """
-    assert os.path.isdir(neb_dir), f"目录{neb_dir}不存在"
-
-    if os.path.exists(os.path.join(neb_dir, "neb.h5")):
-        neb_total = h5py.File(os.path.join(neb_dir, "neb.h5"))
-        # new output (>=2022B)
-        if "/LoopInfo/01/MaxForce" in neb_total.keys():
-            maxforce = np.array(neb_total.get("/LoopInfo/" + image_key + "/MaxForce"))
-        else:  # old output
-            maxforce = np.array(neb_total.get("/Iteration/" + image_key + "/MaxForce"))
-
-        if "/LoopInfo/01/TotalEnergy" in neb_total.keys():  # new output (>=2022B)
-            total_energy = np.array(
-                neb_total.get("/LoopInfo/" + image_key + "/TotalEnergy")
-            )
-        else:  # old output
-            total_energy = np.array(
-                neb_total.get("/Iteration/" + image_key + "/TotalEnergy")
-            )
-
-    elif os.path.exists(os.path.join(neb_dir, "neb.json")):
-        with open(os.path.join(neb_dir, "neb.json"), "r") as fin:
-            neb_total = json.load(fin)
-        if "LoopInfo" in neb_total.keys():
-            neb = neb_total["LoopInfo"][image_key]
-        else:
-            neb = neb_total["Iteration"][image_key]
-        maxforce = []
-        total_energy = []
-        for n in neb:
-            maxforce.append(n["MaxForce"])
-            total_energy.append(n["TotalEnergy"])
-
-        maxforce = np.array(maxforce)
-        total_energy = np.array(total_energy)
-
-    else:
-        print(
-            f"请检查{os.path.join(neb_dir, 'neb.h5')}或{os.path.join(neb_dir, 'neb.h5')}是否都存在！"
-        )
-
-    x = np.arange(len(maxforce))
-
-    force = maxforce
-    energy = total_energy
-
-    if raw:
-        pd.DataFrame({"x": x, "force": force, "energy": energy}).to_csv(
-            "neb_conv.csv", index=False
-        )
-
-    fig = plt.figure()
-    ax1 = fig.add_subplot(111)
-    ax1.plot(x, force, label="Max Force", c="black")
-    ax1.set_xlabel("Number of ionic step")
-    ax1.set_ylabel("Force (eV/Å)")
-    ax2 = ax1.twinx()
-    ax2.plot(x, energy, label="Energy", c="r")
-    ax2.set_xlabel("Number of ionic step")
-    ax2.set_ylabel("Energy (eV)")
-    ax2.ticklabel_format(useOffset=False)  # y轴坐标显示绝对值而不是相对值
-    fig.legend(loc=1, bbox_to_anchor=(1, 1), bbox_transform=ax1.transAxes)
-
-    plt.tight_layout()
-    # save and show
-    if figname:
-        if os.path.dirname(figname):  # not just a file name
-            os.makedirs(os.path.dirname(figname), exist_ok=True)
-        plt.savefig(figname)
-        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
-    if show:
-        plt.show()
-
-    return ax1, ax2
-
-
-def printef(directory):
-    """打印NEB计算时各构型的能量和受力
-
-    Parameters
-    ----------
-    directory : str
-        NEB计算的目录，默认为当前目录
-
-    Returns
-    -------
-    打印各构型的能量和受力
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.nebtools import printef
-    >>> printef(directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
-        Force(eV/Å)     RC(Å)    Energy(eV)  E-E0(eV)
-    00     0.180272  0.000000 -39637.098409  0.000000
-    01     0.026337  0.542789 -39637.018595  0.079814
-    02     0.024798  1.086800 -39636.880144  0.218265
-    03     0.234429  1.588367 -39636.998366  0.100043
-    04     0.014094  2.089212 -39637.089994  0.008414
-    """
-    subfolders, resort_mfs, rcs, ens, dEs = _getef(directory)
-    data = np.array([resort_mfs, rcs, ens, dEs], dtype=float)
-    df = pd.DataFrame(
-        data.T,
-        columns=["Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
-        index=subfolders,
-    )
-    print(df)
-
-
-def restart(directory: str = ".", output: str = "bakfile"):
-    """将旧NEB任务归档压缩，并在原路径下准备续算
-
-    Parameters
-    ----------
-    directory : str
-        旧NEB任务所在路径，默认当前路径
-    output : str
-        备份文件夹路径，默认将在当前路径新建一个bakfile文件夹用于备份；
-        也可以任意指定一个路径，但不能与当前路径相同
-
-    Examples
-    ----------
-    >>> from dspawpy.diffusion.nebtools import restart
-    >>> restart(directory='/data/home/hzw1002/dspawpy_repo/test/neb_temp_back', output='/data/home/hzw1002/dspawpy_repo/test/out/neb_backup')
-    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/00压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/00.zip
-    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/01压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/01.zip
-    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/02压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/02.zip
-    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/03压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/03.zip
-    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/04压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/04.zip
-    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/tmp压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/neb_data.zip
-
-    续算准备工作可能需要较长时间才能完成，请耐心等待
-    """
-    while True:
-        if os.path.isdir(output):
-            if os.path.abspath(output) == os.getcwd():
-                raise ValueError("备份文件夹不能与当前路径相同！")
-            else:
-                output += "_new"
-                continue
-        else:
-            break
-
-    subfolders = get_neb_subfolders(directory, return_abs=True)  # 获取子文件夹路径
-    os.makedirs(output, exist_ok=True)  # 创建bakfile文件夹
-    # 先处理子文件夹00，01...
-    for subfolder_old in subfolders:
-        folder_index = subfolder_old.split("/")[-1]  # 00，01...
-        subfolder_back = os.path.join(output, folder_index)  # 子文件夹备份到此
-        shutil.move(subfolder_old, subfolder_back)
-        os.makedirs(subfolder_old, exist_ok=True)  # 原文件夹清空了
-
-        latestStructureFile = f"{subfolder_back}/latestStructure{folder_index}.as"
-        structureFile = f"{subfolder_back}/structure{folder_index}.as"
-
-        # 将结构文件复制到原路径下用于续算，有ls则用之，否则用s代替，都没有则报错
-        s_in_old = f"{subfolder_old}/structure{folder_index}.as"
-        if os.path.isfile(latestStructureFile):
-            shutil.copy(latestStructureFile, s_in_old)
-        elif os.path.isfile(structureFile):
-            print(f"未找到{latestStructureFile}，复用{structureFile}续算")
-            shutil.copy(structureFile, s_in_old)
-        else:
-            raise FileNotFoundError(f"{latestStructureFile}和{structureFile}都不存在！")
-
-        # 暂时放到备份主路径下，如果都没有，前面就已经报错了
-        ls_bk = os.path.join(directory, f"latestStructure{folder_index}.as")
-        s_bk = os.path.join(directory, f"structure{folder_index}.as")
-        if os.path.isfile(latestStructureFile):
-            shutil.copy(latestStructureFile, ls_bk)
-        if os.path.isfile(structureFile):
-            shutil.copy(structureFile, s_bk)
-
-        # 处理备份路径下的子文件夹
-        zf = f"{os.path.abspath(output)}/{folder_index}.zip"
-        _zip_folder(subfolder_back, zf)  # 压缩子文件夹
-        # 清空备份子文件夹
-        for file in os.listdir(subfolder_back):
-            os.remove(os.path.join(subfolder_back, file))
-
-        # 将压缩包、结构文件移入
-        shutil.move(zf, f"{subfolder_back}/{folder_index}.zip")
-        if os.path.isfile(ls_bk) and os.path.isfile(s_bk):
-            shutil.move(ls_bk, f"{subfolder_back}/latestStructure{folder_index}.as")
-            shutil.move(s_bk, f"{subfolder_back}/structure{folder_index}.as")
-        elif os.path.isfile(ls_bk):
-            shutil.move(ls_bk, f"{subfolder_back}/latestStructure{folder_index}.as")
-        elif os.path.isfile(s_bk):
-            shutil.move(s_bk, f"{subfolder_back}/structure{folder_index}.as")
-        else:
-            raise FileNotFoundError(f"{ls_bk}和{s_bk}都不存在！")
-
-    # 再处理老NEB文件夹主目录下的单个文件
-    # 备份neb.h5,neb.json和DS-PAW.log
-    tmp_dir = os.path.join(output, "tmp")
-    os.makedirs(tmp_dir, exist_ok=True)
-    if os.path.isfile(f"{directory}/neb.h5"):
-        shutil.move(f"{directory}/neb.h5", f"{tmp_dir}/neb.h5")
-    else:
-        print("未找到neb.h5，将不会备份")
-
-    if os.path.isfile(f"{directory}/neb.json"):
-        shutil.move(f"{directory}/neb.json", f"{tmp_dir}/neb.json")
-    else:
-        print("未找到neb.json，将不会备份")
-
-    if len(os.listdir(tmp_dir)) > 0:  # 如果有数据文件
-        _zip_folder(tmp_dir, f"{output}/neb_data.zip")
-        for f in os.listdir(tmp_dir):
-            os.remove(os.path.join(tmp_dir, f))
-        os.removedirs(tmp_dir)
-
-    if os.path.isfile(f"{directory}/DS-PAW.log"):
-        shutil.move(f"{directory}/DS-PAW.log", f"{output}/DS-PAW.log")
-    else:
-        print("未找到DS-PAW.log，将不会备份")
-
-
-def set_pbc(spo):
-    """根据周期性边界条件将分数坐标分量移入 [-0.5, 0.5) 区间
-
-    Parameters
-    ----------
-    spo : np.ndarray or list
-        分数坐标列表
-
-    Returns
-    -------
-    pbc_spo : np.ndarray
-        符合周期性边界条件的分数坐标列表
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.nebtools import set_pbc
-    >>> set_pbc([-0.6, 1.2, 2.3])
-    array([0.4, 0.2, 0.3])
-    """
-    # wrap into [-0.5, 0.5)
-    pbc_spo = np.mod(np.array(spo) + 0.5, 1.0) - 0.5
-
-    return pbc_spo
-
-
-def summary(
-    directory: str = ".", raw=False, show_converge=False, outdir: str = None, **kwargs
-):
-    r"""NEB任务完成总结，依次执行以下步骤：
-
-    - 1. 打印各构型受力、反应坐标、能量、与初始构型的能量差
-    - 2. 绘制能垒图
-    - 3. 绘制并保存结构优化过程的能量和受力收敛过程图
-
-    Parameters
-    ----------
-    directory : str
-        NEB路径, 默认当前路径
-    raw : bool
-        是否保存原始数据到csv文件
-    show_converge : bool
-        是否展示结构优化过程的能量和受力收敛过程图，默认不展示
-    outdir : str
-        收敛过程图保存路径，默认为directory
-    **kwargs : dict
-        传递给plot_barrier的参数
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.nebtools import summary
-    >>> directory = '/data/home/hzw1002/dspawpy_repo/test/2.15' # NEB计算路径，默认当前路径
-    >>> summary(directory, show=False)
-    --> 1. 打印NEB计算时各构型的能量和受力...
-        Force(eV/Å)     RC(Å)    Energy(eV)  E-E0(eV)
-    00     0.180272  0.000000 -39637.098409  0.000000
-    01     0.026337  0.542789 -39637.018595  0.079814
-    02     0.024798  1.086800 -39636.880144  0.218265
-    03     0.234429  1.588367 -39636.998366  0.100043
-    04     0.014094  2.089212 -39637.089994  0.008414
-    <BLANKLINE>
-    --> 2. 绘制能垒图...
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/dspawpy/neb_barrier.png
-    <BLANKLINE>
-    --> 3. 绘制收敛过程图到各构型文件夹中...
-    ----> /data/home/hzw1002/dspawpy_repo/test/2.15/01/converge.png...
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/2.15/01/converge.png
-    ----> /data/home/hzw1002/dspawpy_repo/test/2.15/02/converge.png...
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/2.15/02/converge.png
-    ----> /data/home/hzw1002/dspawpy_repo/test/2.15/03/converge.png...
-    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/2.15/03/converge.png
-    <BLANKLINE>
-    完成!
-
-    若inifin=false，用户必须将自洽的scf.h5或system.json放到初末态子文件夹中
-    """
-    # 1. 绘制能垒图
-    print("--> 1. 打印NEB计算时各构型的能量和受力...")
-    printef(directory)
-
-    # 2. 打印各构型受力、反应坐标、能量、与初始构型的能量差
-    print("\n--> 2. 绘制能垒图...")
-    plt.clf()  # 清空画布再画图
-    plot_barrier(directory=directory, raw=raw, **kwargs)
-
-    # 3. 绘制并保存结构优化过程的能量和受力收敛过程图到各构型文件夹中
-    print("\n--> 3. 绘制收敛过程图到各构型文件夹中...")
-    subfolders = get_neb_subfolders(directory)
-    for subfolder in subfolders[1 : len(subfolders) - 1]:
-        if outdir:
-            os.makedirs(os.path.join(outdir, subfolder), exist_ok=True)
-            pngfile = f"{outdir}/{subfolder}/converge.png"
-        else:
-            pngfile = f"{directory}/{subfolder}/converge.png"
-
-        print(f"----> {pngfile}...")
-        plot_neb_converge(
-            neb_dir=directory,
-            image_key=subfolder,
-            figname=pngfile,
-            raw=raw,
-            show=show_converge,
-        )
-    plt.clf()
-    print("\n完成!")
-
-
-def write_movie_json(preview: bool = False, directory: str = ".", step: int = -1):
-    r"""NEB计算或者初始插值后，读取信息，保存为 neb_movie*.json 文件
-
-    用 Device Studio 打开该文件可以观察结构等信息
-
-    Parameters
-    ----------
-    preview : bool
-        是否预览模式，默认否
-    directory : str
-        计算结果所在目录. 默认当前路径
-    step: int
-        离子步编号. 默认-1，读取整个NEB计算过程信息。
-        0表示初插结构（未完成离子步）；
-        1表示第一个离子步，以此类推。
-
-    Returns
-    ----------
-    neb_movie*.json文件
-
-    Examples
-    ----------
-    >>> from dspawpy.diffusion.nebtools import write_movie_json
-
-    NEB计算完成后要观察轨迹变化全过程，只需指定NEB计算路径即可
-
-    >>> write_movie_json(directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
-    正在读取最后一个离子步信息...
-    --> /data/home/hzw1002/dspawpy_repo/dspawpy/neb_movie_last.json 写入成功！
-
-    NEB计算完成后要观察第n离子步结构，请设置step为n，注意step从1开始计数
-
-    >>> write_movie_json(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', step=1)
-    正在读取第1个离子步信息...
-    --> /data/home/hzw1002/dspawpy_repo/dspawpy/neb_movie_1.json 写入成功！
-
-    如果您指定的step数超过NEB实际完成的离子步，将会自动修改为最后一步，实际效果等同于上一行代码
-
-    >>> write_movie_json(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', step=10)
-    正在读取第10个离子步信息...
-    --> /data/home/hzw1002/dspawpy_repo/dspawpy/neb_movie_10.json 写入成功！
-
-    另外，如需预览初插结构，请将preview设置为True，并将directory指定为NEB计算主路径
-
-    >>> write_movie_json(preview=True, directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
-    正在根据初插结构保存neb_movie_init.json...
-    --> /data/home/hzw1002/dspawpy_repo/dspawpy/neb_movie_init.json 写入成功！
-    """
-
-    if preview:  # preview mode, write neb_movie_init.json from structure.as
-        print("正在根据初插结构保存neb_movie_init.json...")
-        try:
-            raw = _from_structures(directory)
-        except FileNotFoundError:
-            print("未找到初始插值结构！")
-        except Exception as e:
-            print("初始插值结构读取失败！", e)
-    else:
-        if step == 0:  # try preview mode to save time
-            try:
-                raw = _from_structures(directory)
-            except FileNotFoundError:
-                print("未找到初始插值结构，将从计算结果h5或json文件中读取！")
-            except Exception as e:
-                print("初始插值结构读取失败！", e)
-        else:
-            try:  # read from h5 file
-                raw = _from_h5(directory, step)
-            except FileNotFoundError:
-                try:  # read from json file
-                    raw = _from_json(directory, step)
-                except json.decoder.JSONDecodeError:
-                    print("json文件格式错误！")
-                except Exception as e:
-                    print(e)
-            except Exception as e:
-                print("h5文件内容读取失败！", e)
-    _dump_neb_movie_json(raw)
-
-
-def write_xyz(preview: bool = False, directory: str = ".", step: int = -1):
-    """
-    将NEB结构链条写成xyz轨迹文件用于可视化
-
-    Parameters
-    ----------
-    preview : bool
-        是否预览模式，默认否
-    directory : str
-        计算结果所在目录. 默认当前路径
-    step: int
-        离子步编号. 默认-1，读取整个NEB计算过程信息。
-        0表示初插结构（未完成离子步）；
-        1表示第一个离子步，以此类推。
-
-    Returns
-    ----------
-    neb_movie.xyz文件
-
-    Examples
-    ----------
-    >>> from dspawpy.diffusion.nebtools import write_xyz
-    >>> write_xyz(directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
-    正在读取最后一个离子步信息...
-    --> /data/home/hzw1002/dspawpy_repo/dspawpy/neb_movie_last.xyz 写入成功！
-    <BLANKLINE>
-    """
-
-    if preview:  # preview mode, write neb_movie_init.xyz from structure.as
-        print("正在根据初插结构保存neb_movie_init.xyz...")
-        try:
-            raw = _from_structures(directory)
-        except FileNotFoundError:
-            print("未找到初始插值结构！")
-        except Exception as e:
-            print("初始插值结构读取失败！", e)
-    else:
-        if step == 0:  # try preview mode to save time
-            try:
-                raw = _from_structures(directory)
-            except FileNotFoundError:
-                print("未找到初始插值结构，将从计算结果h5或json文件中读取！")
-            except Exception as e:
-                print("初始插值结构读取失败！", e)
-        else:
-            try:  # read from h5 file
-                raw = _from_h5(directory, step)
-            except FileNotFoundError:
-                try:  # read from json file
-                    raw = _from_json(directory, step)
-                except json.decoder.JSONDecodeError:
-                    print("json文件格式错误！")
-                except Exception as e:
-                    print(e)
-            except Exception as e:
-                print("h5文件内容读取失败！", e)
-    _dump_neb_xyz(raw)
-
-
-def _dump_neb_xyz(raw):
-    """根据之前收集到的各数据列表，dump json文件到output"""
-    (
-        output,
-        subfolders,
-        step,
-        MaxForces,
-        TotalEnergies,
-        Poses,  # Nimage x Natom x 3 , read
-        Latvs,  # Nimage x 9
-        Elems,  # Nimage x Natom
-        Fixs,  # Natom x 3
-        reactionCoordinates,
-        totalEnergies,
-        maxForces,
-        tangents,
-        iDirects,
-    ) = raw
-
-    # 写入文件
-    xyzfile = output[:-5] + ".xyz"
-    Nstep = len(subfolders)  # 选定离子步，展示构型链
-    with open(xyzfile, "w") as f:
-        # Nstep
-        for n in range(Nstep):
-            eles = Elems[n]  # 针对每个构型
-            # 原子数不会变，就是不合并的元素总数
-            f.write("%d\n" % len(eles))
-            # lattice
-            f.write(
-                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
-                % (
-                    Latvs[n, 0],
-                    Latvs[n, 1],
-                    Latvs[n, 2],
-                    Latvs[n, 3],
-                    Latvs[n, 4],
-                    Latvs[n, 5],
-                    Latvs[n, 6],
-                    Latvs[n, 7],
-                    Latvs[n, 8],
-                )
-            )
-            # position and element
-            for i in range(len(eles)):
-                f.write(
-                    "%s %f %f %f\n"
-                    % (eles[i], Poses[n, i, 0], Poses[n, i, 1], Poses[n, i, 2])
-                )
-    print(f"--> {os.path.abspath(xyzfile)} 写入成功！\n")
-
-
-def _from_structures(directory: str):
-    """从structure00.as，structure01.as，...，中读取结构信息，
-    写入neb_movie_init，以便用DeviceStudio打开观察
-
-    Parameters
-    ----------
-    directory : str
-        NEB计算路径，默认当前路径
-
-    Returns
-    -------
-    用于json文件的各个数组
-    """
-    output = "neb_movie_init.json"
-    step = 0
-
-    subfolders = get_neb_subfolders(directory)
-    # print(subfolders)
-    nimage = len(subfolders)
-    reactionCoordinates = np.zeros(shape=nimage)  # optional
-    totalEnergies = np.zeros(shape=nimage)  # optional
-    maxForces = np.zeros(shape=nimage - 2)  # optional
-    tangents = np.zeros(shape=nimage - 2)  # optional
-    MaxForces = np.zeros(shape=(nimage - 2, step + 1))  # optional
-    TotalEnergies = np.zeros(shape=(nimage - 2, step + 1))  # optional
-
-    Poses = []  # nimage x Natom x 3 , read
-    Elems = []  # nimage x Natom, read
-    Latvs = []  # nimage x 9, read
-
-    iDirects = []  # read coordinate type
-    for i, folder in enumerate(subfolders):
-        structure_path = os.path.join(directory, folder, f"structure{folder}.as")
-        if not os.path.exists(structure_path):
-            raise FileNotFoundError(f"请检查{structure_path}是否存在！")
-        structure = build_Structures_from_datafile(structure_path)[0]
-        pos = structure.cart_coords
-        ele = [str(i) for i in structure.species]
-        lat = structure.lattice.matrix
-        Poses.append(pos)
-        Elems.append(ele)
-        Latvs.append(lat)
-        with open(structure_path, "r") as f:
-            lines = f.readlines()
-            coordinateType = lines[6].split()[0]
-            if coordinateType == "Direct":
-                iDirect = True
-            elif coordinateType == "Cartesian":
-                iDirect = False
-            else:
-                raise ValueError(f"请检查{structure_path}中的坐标类型！")
-            iDirects.append(iDirect)
-    Natom = len(Elems[0])
-
-    # reshape data
-    Poses = np.array(Poses).reshape((nimage, Natom, 3))
-    Elems = np.array(Elems).reshape((nimage, Natom))
-    Latvs = np.array(Latvs).reshape((nimage, 9))
-    Fixs = np.zeros(shape=(Natom, 3))  # optional
-
-    return (
-        output,
-        subfolders,
-        step,
-        MaxForces,
-        TotalEnergies,
-        Poses,
-        Latvs,
-        Elems,
-        Fixs,
-        reactionCoordinates,
-        totalEnergies,
-        maxForces,
-        tangents,
-        iDirects,
-    )
-
-
-def _from_h5(directory: str, step: int):
-    """从NEB路径下的h5文件读取 从第一步开始到指定step数 的结构和能量信息，
-    写入json文件，以便用DeviceStudio打开观察。
-
-    支持热读取结构信息（其他信息忽略）
-
-    Parameters
-    ----------
-    directory : str
-        NEB路径，默认当前路径
-    step : int
-        step数，默认-1，读取最后一个构型
-
-    Returns
-    -------
-    用于json文件的各个数组
-    """
-    # ^ 前期设置
-    neb_h5 = os.path.join(directory, "01", "neb01.h5")
-    ele = get_ele_from_h5(hpath=neb_h5)
-    Natom = len(ele)
-    data = h5py.File(neb_h5)
-    try:
-        total_steps = np.array(data.get("/NebSize"))[0]
-    except:
-        print("NEB计算未正常结束，正在尝试实时读取结构信息...")
-        try:
-            total_steps = np.array(data.get("/Structures/FinalStep"))[0]
-        except:
-            raise ValueError("尚未完成第一个离子步，请检查计算是否出错，否则请耐心等待离子步完成至少一个后再尝试读取！")
-
-    if step == -1:
-        output = "neb_movie_last.json"
-        step = total_steps
-        print("正在读取最后一个离子步信息...")
-    elif step > total_steps:
-        output = "neb_movie_last.json"
-        step = total_steps
-        print(f"指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
-        print("正在读取最后一个离子步信息...")
-    else:
-        output = "neb_movie_{}.json".format(step)
-        print(f"正在读取第{step}个离子步信息...")
-
-    # ^ 读取前，准备好json文件所需数组框架
-    subfolders = get_neb_subfolders(directory)
-    nimage = len(subfolders)
-    reactionCoordinates = np.zeros(shape=nimage)  # optional
-    totalEnergies = np.zeros(shape=nimage)  # optional，每个构型最终能量
-    maxForces = np.zeros(shape=nimage - 2)  # optional
-    tangents = np.zeros(shape=nimage - 2)  # optional
-    MaxForces = np.zeros(shape=(nimage - 2, step))  # optional
-    TotalEnergies = np.zeros(shape=(nimage - 2, step))  # optional，中间构型每个离子步能量
-    # Sposes = []  # nimage x Natom x 3 , read
-    Sposes = np.empty(shape=(nimage, Natom, 3))  # nimage x Natom x 3 , read
-    Elems = []  # nimage x Natom, read
-    Latvs = []  # nimage x 9, read
-    Fixs = []  # Natom x 3, set
-
-    for folder in subfolders:
-        """如果是首尾两个构型，最多只有scf.h5文件，没有neb.h5文件
-        用户如果算NEB的时候，不计算首尾构型的自洽，
-         或者在别处算完了但是没有复制到首尾文件夹中并命名为scf.h5，
-          便不能使用第一个功能
-        """
-        if folder == subfolders[0] or folder == subfolders[-1]:
-            h5_path = os.path.join(directory, folder, "scf.h5")
-            spath = os.path.join(directory, folder, f"structure{folder}.as")
-            assert os.path.exists(h5_path) or os.path.exists(
-                spath
-            ), f"请确认{h5_path}或{spath}至少存在一个！"
-        else:
-            h5_path = os.path.join(directory, folder, f"neb{folder}.h5")
-            assert os.path.exists(h5_path), f"请确认{h5_path}是否存在！"
-
-    # ^ 开始分功能读取数据
-    for i, folder in enumerate(subfolders):
-        if folder == subfolders[0] or folder == subfolders[-1]:
-            h5_path = os.path.join(directory, folder, "scf.h5")
-            if os.path.exists(h5_path):
-                data = h5py.File(h5_path)
-                # 不影响可视化，直接定为0
-                if folder == subfolders[0]:
-                    reactionCoordinates[i] = 0
-                pos = np.array(data.get("/Structures/Step-1/Position")).reshape(
-                    -1, 3
-                )  # scaled
-                lat = np.array(data.get("/Structures/Step-1/Lattice"))
-                ele = get_ele_from_h5(hpath=h5_path)
-                totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
-            else:
-                structure = build_Structures_from_datafile(spath)[0]
-                pos = structure.frac_coords
-                ele = [str(i) for i in structure.species]
-                lat = structure.lattice.matrix
-        else:
-            h5_path = os.path.join(directory, folder, f"neb{folder}.h5")
-            data = h5py.File(h5_path)
-            # reading...
-            try:
-                reactionCoordinates[i - 1] = np.array(data.get("/Distance/Previous"))[
-                    -1
-                ]
-                maxForces[i - 1] = np.array(data.get("/MaxForce"))[-1]
-                tangents[i - 1] = np.array(data.get("/Tangent"))[-1]
-                if folder == subfolders[-2]:
-                    reactionCoordinates[i + 1] = np.array(data.get("/Distance/Next"))[
-                        -1
-                    ]
-                # read MaxForces and TotalEnergies
-                nionStep = np.array(data.get("/MaxForce")).shape[0]
-                assert step <= nionStep, f"总共只完成了{nionStep}个离子步!"
-                for j in range(step):
-                    MaxForces[i - 1, j] = np.array(data.get("/MaxForce"))[j]
-                    TotalEnergies[i - 1, j] = np.array(data.get("/TotalEnergy"))[j]
-                totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
-            except:
-                pass  # 还没完成NEB计算，不影响读取结构信息用于可视化
-            # read the latest structure for visualization
-            pos = np.array(data.get(f"/Structures/Step-{step}/Position")).reshape(
-                Natom, 3
-            )  # scaled
-            lat = np.array(data.get(f"/Structures/Step-{step}/Lattice"))
-            ele = get_ele_from_h5(hpath=h5_path)
-
-        Elems.append(ele)
-        Sposes[i, :, :] = pos
-        Latvs.append(lat)
-
-    if os.path.exists(os.path.join(directory, "neb.h5")):
-        tdata = h5py.File(os.path.join(directory, "neb.h5"))
-        # atom fix, not lattice
-        # ignore this trivial message because it is not necessary for the visualization
-        if "/UnrelaxStructure/Image00/Fix" in tdata:
-            fix_array = np.array(tdata.get("/UnrelaxStructure/Image00/Fix"))
-            for fix in fix_array:
-                if fix == 0.0:
-                    F = False
-                elif fix == 1.0:
-                    F = True
-                else:
-                    raise ValueError("Fix值只能为0或1")
-                Fixs.append(F)
-        else:
-            Fixs = np.full(shape=(Natom, 3), fill_value=False)
-    else:
-        Fixs = np.full(shape=(Natom, 3), fill_value=False)
-
-    Elems = np.array(Elems).reshape((nimage, Natom))
-    Latvs = np.array(Latvs).reshape((nimage, 9))
-    Fixs = np.array(Fixs).reshape((Natom, 3))
-    iDirects = [True for i in range(Natom)]  # only output direct coordinates
-
-    return (
-        output,
-        subfolders,
-        step,
-        MaxForces,
-        TotalEnergies,  #
-        Sposes,
-        Latvs,
-        Elems,
-        Fixs,
-        reactionCoordinates,
-        totalEnergies,
-        maxForces,
-        tangents,
-        iDirects,
-    )
-
-
-def _from_json(directory: str, step: int):
-    """从NEB路径下的json文件读取 从第一步开始到指定step数 的结构和能量信息，
-    写入json文件，以便用DeviceStudio打开观察
-
-    Parameters
-    ----------
-    directory : str
-        NEB路径，默认当前路径
-    step : int
-        step数，默认-1，读取最后一个构型
-
-    Returns
-    -------
-    用于json文件的各个数组
-    """
-
-    # ^ 前期设置
-    neb_js = os.path.join(directory, "01/neb01.json")
-    with open(neb_js, "r") as f:
-        data = json.load(f)
-    total_steps = len(data)
-
-    if step == -1:
-        output = "neb_movie_last.json"
-        step = total_steps
-        print("正在读取最后一个离子步信息（h5文件不存在，尝试从json文件读取数据）...")
-    elif step > total_steps:
-        output = "neb_movie_last.json"
-        step = total_steps
-        print(f"您指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
-        print("正在读取最后一个离子步信息（h5文件不存在，尝试从json文件读取数据）...")
-    else:
-        output = f"neb_movie_{step}.json"
-        print(f"正在读取第{step}个离子步信息...")
-
-    # ^ 读取前，准备好json文件所需数组框架
-    subfolders = get_neb_subfolders(directory)
-    nimage = len(subfolders)
-    reactionCoordinates = np.zeros(shape=nimage)  # optional
-    totalEnergies = np.zeros(shape=nimage)  # optional，每个构型最终能量
-    maxForces = np.zeros(shape=nimage - 2)  # optional
-    tangents = np.zeros(shape=nimage - 2)  # optional
-    MaxForces = np.zeros(shape=(nimage - 2, step))  # optional
-    TotalEnergies = np.zeros(shape=(nimage - 2, step))  # optional，中间构型每个离子步能量
-    Sposes = []  # nimage x Natom x 3 , read
-    Elems = []  # nimage x Natom, read
-    Latvs = []  # nimage x 9, read
-    Fixs = []  # Natom x 3, set
-
-    for folder in subfolders:
-        """如果是首尾两个构型，最多只有system.json文件，没有neb*.json文件
-        用户如果算NEB的时候，不计算首尾构型的自洽，
-         或者在别处算完了但是没有复制到首尾文件夹中并命名为system.json，
-          便不能使用第一个功能
-        """
-        if folder == subfolders[0] or folder == subfolders[-1]:
-            js_path = os.path.join(directory, folder, "system.json")
-        else:
-            js_path = os.path.join(directory, folder, f"neb{folder}.json")
-        assert os.path.exists(js_path), f"请确认{js_path}是否存在！"
-
-    # ^ 开始分功能读取数据
-    for i, folder in enumerate(subfolders):
-        if i == 0:  # 初末态在NEB计算过程中不会优化结构
-            # 1. 外部自洽后移动system.json
-            js_path = os.path.join(directory, folder, "system.json")
-            # 2. 直接NEB计算，得到system00.json
-            neb_js_path = os.path.join(directory, folder, f"system{folder}.json")
-            if os.path.exists(neb_js_path):  # 优先读取neb计算得到的system00.json
-                with open(neb_js_path, "r") as f:
-                    data = json.load(f)
-
-            elif os.path.exists(js_path):
-                with open(js_path, "r") as f:
-                    data = json.load(f)
-
-            else:
-                raise FileNotFoundError(
-                    f"{os.path.abspath(js_path)}和{os.path.abspath(neb_js_path)}均不存在！"
-                )
-
-            lat = data["AtomInfo"]["Lattice"]
-            Latvs.append(lat)
-
-            Natom = len(data["AtomInfo"]["Atoms"])  # 读取原子数
-            for j in range(Natom):
-                pos = data["AtomInfo"]["Atoms"][j]["Position"]  # scaled
-                Sposes.append(pos)
-
-            totalEnergies[i] = data["Energy"]["TotalEnergy0"]
-            reactionCoordinates[i] = 0.0
-
-        elif i > 0 and i < nimage - 1:  # 中间构型会优化结构
-            # 读取晶胞矢量、原子坐标
-            relax_json = os.path.join(directory, folder, "relax.json")
-            assert os.path.exists(relax_json), f"{relax_json}不存在！"
-
-            with open(relax_json, "r") as f:
-                rdata = json.load(f)
-
-            lat = rdata[step - 1]["Lattice"]  # 第step步优化后的晶胞
-            Latvs.append(lat)
-
-            Natom = len(rdata[0]["Atoms"])
-            for j in range(Natom):  # for each atom
-                pos = rdata[step - 1]["Atoms"][j]["Position"]  # 第step步优化后的原子坐标
-                Sposes.append(pos)  # ! 输出的都是分数坐标
-
-            # 读取能量和反应坐标
-            nj = os.path.join(directory, folder, f"neb{folder}.json")
-            with open(nj, "r") as f:
-                print(f"Reading {os.path.abspath(nj)}...")
-                ndata = json.load(f)
-
-            totalEnergies[i] = ndata[step - 1]["TotalEnergy"]  # 读取第step步优化后的能量
-
-            # 读取与前一个构型相比的反应坐标
-            reactionCoordinates[i - 1] = ndata[step - 1]["ReactionCoordinate"][-2]
-            tangents[i - 1] = ndata[step - 1]["Tangent"]
-            if folder == subfolders[-2]:  # 末态前一个构型的计算结果中读取反应坐标
-                reactionCoordinates[i + 1] = ndata[step - 1]["ReactionCoordinate"][-1]
-            for j in range(step):
-                MaxForces[i - 1, j] = ndata[j]["MaxForce"]
-                # neb01.json中不存在TotalEnergy0，暂时读取TotalEnergy
-                TotalEnergies[i - 1, j] = ndata[j]["TotalEnergy"]
-
-        else:  # 末态构型
-            js_path = os.path.join(directory, folder, "system.json")
-            neb_js_path = os.path.join(directory, folder, f"system{folder}.json")
-            if os.path.exists(neb_js_path):  # 优先读取neb计算得到的json文件
-                with open(neb_js_path, "r") as f:
-                    data = json.load(f)
-
-            elif os.path.exists(js_path):
-                with open(js_path, "r") as f:
-                    data = json.load(f)
-
-            else:
-                raise FileNotFoundError(
-                    f"{os.path.abspath(js_path)}和{os.path.abspath(neb_js_path)}均不存在！"
-                )
-
-            lat = data["AtomInfo"]["Lattice"]
-            Latvs.append(lat)
-
-            Natom = len(data["AtomInfo"]["Atoms"])  # 读取原子数
-            for j in range(Natom):
-                pos = data["AtomInfo"]["Atoms"][j]["Position"]  # scaled
-                Sposes.append(pos)
-
-            energy = data["Energy"]["TotalEnergy0"]
-            totalEnergies[i] = energy
-
-    # 读取原子元素
-    tneb_js = os.path.join(directory, "neb.json")
-    with open(tneb_js, "r") as f:
-        tdata = json.load(f)
-
-    Natom = len(tdata["UnrelaxStructure"][0]["Atoms"])
-    elems = []
-    for k in range(Natom):
-        ele = tdata["UnrelaxStructure"][0]["Atoms"][k]["Element"]
-        elems.append(ele)
-
-    for ni in range(nimage):
-        Elems.append(elems)  # 重复nimage次，保持Elems结构一致
-
-    for atom in range(Natom):
-        fix_array = tdata["UnrelaxStructure"][1]["Atoms"][atom]["Fix"]  # (1,3)
-        if fix_array == []:  # empty list
-            fix_array = [0.0, 0.0, 0.0]
-        for fix in fix_array:
-            if fix == 0.0:
-                F = False
-            elif fix == 1.0:
-                F = True
-            else:
-                raise ValueError("Fix值只能为 0.0 或 1.0")
-            Fixs.append(F)
-
-    # 累加reactionCoordinates中的元素
-    for i in range(1, len(reactionCoordinates)):
-        reactionCoordinates[i] += reactionCoordinates[i - 1]
-
-    # reshape data
-    Sposes = np.array(Sposes).reshape((nimage, Natom, 3))
-    Elems = np.array(Elems).reshape((nimage, Natom))
-    Latvs = np.array(Latvs).reshape((nimage, 9))
-    Fixs = np.array(Fixs).reshape((Natom, 3))
-    iDirects = [True for i in range(Natom)]  # only output direct coordinates
-
-    return (
-        output,
-        subfolders,
-        step,
-        MaxForces,
-        TotalEnergies,
-        Sposes,
-        Latvs,
-        Elems,
-        Fixs,
-        reactionCoordinates,
-        totalEnergies,
-        maxForces,
-        tangents,
-        iDirects,
-    )
-
-
-def _dump_neb_movie_json(raw):
-    """根据之前收集到的各数据列表，dump json文件到output"""
-    (
-        output,
-        subfolders,
-        step,
-        MaxForces,
-        TotalEnergies,
-        Poses,
-        Latvs,
-        Elems,
-        Fixs,
-        reactionCoordinates,
-        totalEnergies,
-        maxForces,
-        tangents,
-        iDirects,
-    ) = raw
-
-    IterDict = {}
-    for s, sf in enumerate(subfolders):
-        if sf == subfolders[0] or sf == subfolders[-1]:
-            continue
-        else:
-            Eflist = []
-            for l in range(step):
-                ef = {
-                    "MaxForce": MaxForces[s - 1, l],
-                    "TotalEnergy": TotalEnergies[s - 1, l],
-                }
-                Eflist.append(ef)
-                iterDict = {sf: Eflist}  # construct sub-dict
-                IterDict.update(iterDict)  # append sub-dict
-
-    RSList = []
-    """
-    从外到内依次遍历 构型、原子（子字典）
-    原子的键值对为：'Atoms': 原子信息列表
-    原子信息列表是一个由字典组成的列表，每个字典对应一个原子的信息
-    """
-    for s, sf in enumerate(subfolders):
-        pos = Poses[s]
-        lat = Latvs[s]
-        elem = Elems[s]
-        atoms = []
-        for i in range(len(elem)):
-            atom = {
-                "Element": elem[i],
-                "Fix": Fixs[i].tolist(),
-                "Mag": [],  # empty
-                "Position": pos[i].tolist(),
-                "Pot": "",
-            }  # empty
-            atoms.append(atom)
-        if iDirects[s]:
-            rs = {"Atoms": atoms, "CoordinateType": "Direct", "Lattice": lat.tolist()}
-        else:
-            rs = {
-                "Atoms": atoms,
-                "CoordinateType": "Cartesian",
-                "Lattice": lat.tolist(),
-            }
-        RSList.append(rs)
-
-    URSList = []  # DS似乎并不读取这部分信息，空置即可
-
-    data = {
-        "Distance": {"ReactionCoordinate": reactionCoordinates.tolist()},
-        "Energy": {"TotalEnergy": totalEnergies.tolist()},
-        "Force": {"MaxForce": maxForces.tolist(), "Tangent": tangents.tolist()},
-        "Iteration": IterDict,
-        "RelaxedStructure": RSList,
-        "UnrelaxedStructure": URSList,
-    }
-
-    # ^ 将字典写入json文件
-    with open(output, "w") as f:
-        json.dump(data, f, indent=4)
-
-    print(f"--> {os.path.abspath(output)} 写入成功！")
-
-
-def _getef(directory: str = "."):
-    """读取NEB计算时各构型的能量和受力，NEB计算可以未收敛
-    但如果初末态自洽在别处完成，请手动将其移入00等文件夹中！
-
-    Parameters
-    ----------
-    directory: str
-        NEB计算的路径，默认当前路径
-
-    Returns
-    -------
-    subfolders: list
-        构型文件夹名列表
-    resort_mfs: list
-        构型受力的最大分量列表
-    rcs: list
-        反应坐标列表
-    ens: list
-        电子总能列表
-    dEs: list
-        与初始构型的能量差列表
-    """
-
-    subfolders = get_neb_subfolders(directory)
-    Nimage = len(subfolders)
-
-    ens = []
-    dEs = np.zeros(Nimage)
-    rcs = [0]
-    mfs = []
-
-    # read energies
-    count = 1
-    for i, subfolder in enumerate(subfolders):
-        if i == 0 or i == Nimage - 1:
-            jsf = os.path.join(directory, subfolder, f"system{subfolder}.json")
-            old_jsf = os.path.join(directory, subfolder, "system.json")
-            hf = os.path.join(directory, subfolder, "scf.h5")
-
-            if os.path.exists(hf):  # 优先读取h5文件内容
-                data = h5py.File(hf)
-                en = np.array(data.get("/Energy/TotalEnergy0"))
-                if i == 0 or i == Nimage - 1:
-                    mf = np.max(np.abs(np.array(data.get("/Force/ForceOnAtoms"))))
-                    mfs.append(mf)
-
-            elif os.path.exists(jsf):  # 其次读取json文件内容
-                with open(jsf, "r") as f:
-                    data = json.load(f)
-                en = data["Energy"]["TotalEnergy0"]
-                if i == 0 or i == Nimage - 1:
-                    mf = np.max(np.abs(data["Force"]["ForceOnAtoms"]))
-                    mfs.append(mf)
-
-            elif os.path.exists(old_jsf):  # 兼容老json
-                with open(old_jsf, "r") as f:
-                    data = json.load(f)
-                en = data["Energy"]["TotalEnergy0"]
-                if i == 0 or i == Nimage - 1:
-                    mf = np.max(np.abs(data["Force"]["ForceOnAtoms"]))
-                    mfs.append(mf)
-
-            else:
-                raise FileNotFoundError(
-                    "无法找到记录构型%s的能量和受力的system.json或scf.h5文件" % subfolder
-                )
-            ens.append(en)
-
-        else:
-            jsf = os.path.join(directory, subfolder, f"neb{subfolder}.json")
-            sysjsf = os.path.join(directory, subfolder, f"system{subfolder}.json")
-            old_sysjsf = os.path.join(directory, subfolder, "system.json")
-            hf = os.path.join(directory, subfolder, f"neb{subfolder}.h5")
-
-            if os.path.exists(hf):  # 优先读取h5文件内容
-                data = h5py.File(hf)
-                en = np.array(data.get("/Energy/TotalEnergy0"))
-                mf = np.array(data.get("/MaxForce"))[-1]
-                # the key may change depends on your DS-PAW version
-                if "/Distance/Previous" in data:
-                    rc = np.array(data.get("/Distance/Previous"))[-1]
-                elif "/ReactionCoordinate" in data:
-                    rc = np.array(data.get("/ReactionCoordinate"))[-2]
-                else:
-                    raise KeyError("找不到/Distance/Previous或/ReactionCoordinate键！")
-                rcs.append(rc)
-                if count == Nimage - 2:  # before final image
-                    if "/Distance/Next" in data:
-                        rc = np.array(data.get("/Distance/Next"))[-1]
-                    elif "/ReactionCoordinate" in data:
-                        rc = np.array(data.get("/ReactionCoordinate"))[-1]
-                    else:
-                        raise KeyError("找不到/Distance/Next或/ReactionCoordinate键！")
-                    rcs.append(rc)
-
-            elif os.path.exists(jsf):
-                if os.path.exists(sysjsf):
-                    with open(sysjsf, "r") as f:
-                        data = json.load(f)
-                    en = data["Energy"]["TotalEnergy0"]
-                elif os.path.exists(old_sysjsf):  # 兼容旧版DS-PAW
-                    with open(old_sysjsf, "r") as f:
-                        data = json.load(f)
-                    en = data["Energy"]["TotalEnergy0"]
-                else:
-                    raise FileNotFoundError(f"无法找到{sysjsf}或{old_sysjsf}")
-
-                with open(jsf, "r") as f:
-                    data = json.load(f)
-                Nion_step = len(data)
-                # en = data[Nion_step - 1]["TotalEnergy"] # invalid
-                mf = data[Nion_step - 1]["MaxForce"]  # 最后一步的最大受力
-                rc = data[Nion_step - 1]["ReactionCoordinate"][0]  # 最后一步的反应坐标
-                rcs.append(rc)
-                if count == Nimage - 2:  # before final image
-                    rc = data[Nion_step - 1]["ReactionCoordinate"][1]  # 最后一步的反应坐标
-                    rcs.append(rc)
-
-            else:
-                raise FileNotFoundError(f"无法找到{hf}或{jsf}")
-
-            ens.append(en)
-            mfs.append(mf)
-
-            # get dE
-            dE = ens[count] - ens[0]
-            dEs[i] = dE
-            count += 1
-    dEs[-1] = ens[Nimage - 1] - ens[0]
-
-    # rcs 改成累加值
-    for i in range(1, len(rcs)):
-        rcs[i] += rcs[i - 1]
-
-    rcs = np.array(rcs)
-
-    resort_mfs = [mfs[0]]
-    final_mf = mfs[1]
-    for j in range(2, len(mfs)):
-        resort_mfs.append(mfs[j])
-    resort_mfs.append(final_mf)
-
-    return subfolders, resort_mfs, rcs, ens, dEs
+import json
+import os
+import shutil
+
+import h5py
+import numpy as np
+import pandas as pd
+
+np.set_printoptions(suppress=True)  # 不使用科学计数法
+import zipfile
+
+import matplotlib.pyplot as plt
+
+from dspawpy.io.structure import build_Structures_from_datafile
+from dspawpy.io.utils import get_ele_from_h5
+
+
+def _zip_folder(folder_path, output_path):
+    with zipfile.ZipFile(output_path, "w", zipfile.ZIP_DEFLATED) as zipf:
+        for root, _, files in os.walk(folder_path):
+            for file in files:
+                file_path = os.path.join(root, file)
+                zipf.write(file_path, os.path.relpath(file_path, folder_path))
+    print(f"已将{folder_path}压缩到{output_path}")
+
+
+def get_distance(
+    spo1: np.ndarray, spo2: np.ndarray, lat1: np.ndarray, lat2: np.ndarray
+):
+    r"""根据两个结构的分数坐标和晶胞计算距离
+
+    Parameters
+    ----------
+    spo1 : np.ndarray
+        分数坐标列表1
+    spo2 : np.ndarray
+        分数坐标列表2
+    lat1 : np.ndarray
+        晶胞1
+    lat2 : np.ndarray
+        晶胞2
+
+    Returns
+    -------
+    float
+        距离
+
+    Examples
+    --------
+
+    先读取结构信息
+
+    >>> from dspawpy.io.structure import build_Structures_from_datafile
+    >>> s1 = build_Structures_from_datafile('/data/home/hzw1002/dspawpy_repo/test/2.15/01/structure01.as')[0]
+    >>> s2 = build_Structures_from_datafile('/data/home/hzw1002/dspawpy_repo/test/2.15/02/structure02.as')[0]
+
+    计算两个构型的距离
+
+    >>> from dspawpy.diffusion.nebtools import get_distance
+    >>> dist = get_distance(s1.frac_coords, s2.frac_coords, s1.lattice.matrix, s2.lattice.matrix)
+    >>> print('两个构型的距离为：', dist, 'Angstrom')
+    两个构型的距离为： 0.476972808803491 Angstrom
+    """
+    diff_spo = spo1 - spo2  # 分数坐标差
+    avglatv = 0.5 * (lat1 + lat2)  # 平均晶格矢量
+    pbc_diff_spo = set_pbc(diff_spo)  # 笛卡尔坐标差
+    # 分数坐标点乘平均晶胞，转回笛卡尔坐标
+    pbc_diff_pos = np.dot(pbc_diff_spo, avglatv)  # 笛卡尔坐标差
+    distance = np.sqrt(np.sum(pbc_diff_pos**2))
+
+    return distance
+
+
+def get_neb_subfolders(directory: str = ".", return_abs=False):
+    r"""将directory路径下的子文件夹名称列表按照数字大小排序
+
+    仅保留形如00，01数字类型的NEB子文件夹路径
+
+    Parameters
+    ----------
+    subfolders : list
+        子文件夹名称列表
+    return_abs : bool, optional
+        是否返回绝对路径, 默认否
+
+    Returns
+    -------
+    subfolders : list
+        排序后的子文件夹名称列表
+
+    Examples
+    --------
+    >>> from dspawpy.diffusion.nebtools import get_neb_subfolders
+    >>> directory = '/data/home/hzw1002/dspawpy_repo/test/2.15'
+    >>> get_neb_subfolders(directory)
+    ['00', '01', '02', '03', '04']
+    """
+    raw_subfolders = next(os.walk(directory))[1]
+    subfolders = []
+    for subfolder in raw_subfolders:
+        try:
+            assert 0 <= int(subfolder) < 100
+            subfolders.append(subfolder)
+        except:
+            pass
+    subfolders.sort()  # 从小到大排序
+    if return_abs:
+        subfolders = [
+            os.path.abspath(os.path.join(directory, subfolder))
+            for subfolder in subfolders
+        ]
+    return subfolders
+
+
+def plot_barrier(
+    datafile: str = "neb.h5",
+    directory: str = None,
+    ri: float = None,
+    rf: float = None,
+    ei: float = None,
+    ef: float = None,
+    method: str = "PchipInterpolator",
+    figname: str = "neb_barrier.png",
+    show: bool = True,
+    raw=False,
+    **kwargs,
+):
+    r"""调用 scipy.interpolate 插值算法，拟合NEB能垒并绘图
+
+    Parameters
+    ----------
+    datafile: str
+        neb.h5或neb.json文件路径
+    directory : str
+        NEB计算路径
+    ri : float
+        初态反应坐标
+    rf : float
+        末态反应坐标
+    ei : float
+        初态自洽能量
+    ef : float
+        末态自洽能量
+    method : str, optional
+        插值算法, by default 'PchipInterpolator'
+    figname : str, optional
+        能垒图名称, by default 'neb_barrier.png'
+    show : bool, optional
+        是否展示交互界面, by default True
+    raw : bool, optional
+        是否返回原始数据到csv
+
+    Raises
+    ------
+    ImportError
+        指定了scipy.interpolate中不存在的插值算法
+    ValueError
+        传递给插值算法的参数不符合该算法要求
+
+    Examples
+    --------
+    >>> from dspawpy.diffusion.nebtools import plot_barrier
+    >>> import matplotlib.pyplot as plt
+    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='interp1d', kind=2, figname=None, show=False)
+    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='interp1d', kind=3, figname=None, show=False)
+    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='CubicSpline', figname=None, show=False)
+    >>> plot_barrier(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', method='pchip', figname=None, show=False)
+    """
+    if directory is not None:
+        # read data
+        subfolders, resort_mfs, rcs, ens, dEs = _getef(directory)
+
+    elif datafile:
+        assert os.path.exists(datafile), f"文件{datafile}不存在"
+        if datafile.endswith(".h5"):
+            from dspawpy.io.read import load_h5
+
+            neb = load_h5(datafile)
+            if "/BarrierInfo/ReactionCoordinate" in neb.keys():
+                reaction_coordinate = neb["/BarrierInfo/ReactionCoordinate"]
+                energy = neb["/BarrierInfo/TotalEnergy"]
+            else:  # old version
+                reaction_coordinate = neb["/Distance/ReactionCoordinate"]
+                energy = neb["/Energy/TotalEnergy"]
+        elif datafile.endswith(".json"):
+            with open(datafile, "r") as fin:
+                neb = json.load(fin)
+            if "BarrierInfo" in neb.keys():
+                reaction_coordinate = neb["BarrierInfo"]["ReactionCoordinate"]
+                energy = neb["BarrierInfo"]["TotalEnergy"]
+            else:  # old version
+                reaction_coordinate = neb["Distance"]["ReactionCoordinate"]
+                energy = neb["Energy"]["TotalEnergy"]
+        else:
+            raise TypeError("datafile 必须是 .h5 或 .json 文件格式")
+
+        x = []
+        for c in reaction_coordinate:
+            if len(x) > 0:
+                x.append(x[-1] + c)
+            else:
+                x.append(c)
+
+        y = [x - energy[0] for x in energy]
+        # initial and final info
+        if ri is not None:  # add initial reaction coordinate
+            x.insert(0, ri)
+        if rf is not None:  # add final reaction coordinate
+            x.append(rf)
+
+        if ei is not None:  # add initial energy
+            y.insert(0, ei)
+        if ef is not None:  # add final energy
+            y.append(ef)
+
+        rcs = np.array(x)
+        dEs = np.array(y)
+
+        print(f"如果NEB任务不计算初末态的自洽，{datafile}中将缺失相关信息，需要手动输入")
+        os.getcwd()
+
+    else:
+        raise ValueError("请指定datafile或directory！")
+
+    # import scipy interpolater
+    try:
+        interpolate_method = getattr(
+            __import__("scipy.interpolate", fromlist=[method]), method
+        )
+    except:
+        raise ImportError(f"无法找到 scipy.interpolate.{method} 算法！")
+    # call the interpolater to interpolate with given kwargs
+    try:
+        inter_f = interpolate_method(rcs, dEs, **kwargs)
+    except:
+        raise ValueError(f"插值失败，请检查{kwargs}参数设置是否有误！")
+
+    xnew = np.linspace(rcs[0], rcs[-1], 100)
+    ynew = inter_f(xnew)
+
+    if raw:
+        pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv", index=False)
+        pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
+            "raw_interpolated_xy.csv", index=False
+        )
+
+    # plot
+    if kwargs:
+        plt.plot(xnew, ynew, label=method + str(kwargs))
+    else:
+        plt.plot(xnew, ynew, label=method)
+    plt.scatter(rcs, dEs, c="r")
+    plt.xlabel("Reaction Coordinate (Å)")
+    plt.ylabel("Energy (eV)")
+    plt.legend()
+
+    plt.tight_layout()
+    # save and show
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
+    if show:
+        plt.show()
+
+
+def plot_neb_converge(
+    neb_dir: str,
+    image_key: str = "01",
+    show: bool = True,
+    figname: str = "neb_conv.png",
+    raw=False,
+):
+    """指定NEB计算路径，绘制NEB收敛过程图
+
+    Parameters
+    ----------
+    neb_dir : str
+        NEB计算路径
+    image_key : str
+        第几个构型，默认 "01"
+    show : bool
+        是否交互绘图
+    image_name : str
+        NEB收敛图名称，默认 "neb_conv.png"
+    raw : bool
+        是否输出原始数据到csv文件
+
+    Returns
+    -------
+    ax1, ax2 : matplotlib.axes.Axes
+        两个子图的Axes对象
+
+    Examples
+    --------
+    >>> from dspawpy.diffusion.nebtools import plot_neb_converge
+    >>> plot_neb_converge(neb_dir='/data/home/hzw1002/dspawpy_repo/test/2.15', image_key='01', figname='/data/home/hzw1002/dspawpy_repo/test/out/neb_converge1.png',show=False)
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/out/neb_converge1.png
+    (<Axes: xlabel='Number of ionic step', ylabel='Force (eV/Å)'>, <Axes: xlabel='Number of ionic step', ylabel='Energy (eV)'>)
+    """
+    assert os.path.isdir(neb_dir), f"目录{neb_dir}不存在"
+
+    if os.path.exists(os.path.join(neb_dir, "neb.h5")):
+        neb_total = h5py.File(os.path.join(neb_dir, "neb.h5"))
+        # new output (>=2022B)
+        if "/LoopInfo/01/MaxForce" in neb_total.keys():
+            maxforce = np.array(neb_total.get("/LoopInfo/" + image_key + "/MaxForce"))
+        else:  # old output
+            maxforce = np.array(neb_total.get("/Iteration/" + image_key + "/MaxForce"))
+
+        if "/LoopInfo/01/TotalEnergy" in neb_total.keys():  # new output (>=2022B)
+            total_energy = np.array(
+                neb_total.get("/LoopInfo/" + image_key + "/TotalEnergy")
+            )
+        else:  # old output
+            total_energy = np.array(
+                neb_total.get("/Iteration/" + image_key + "/TotalEnergy")
+            )
+
+    elif os.path.exists(os.path.join(neb_dir, "neb.json")):
+        with open(os.path.join(neb_dir, "neb.json"), "r") as fin:
+            neb_total = json.load(fin)
+        if "LoopInfo" in neb_total.keys():
+            neb = neb_total["LoopInfo"][image_key]
+        else:
+            neb = neb_total["Iteration"][image_key]
+        maxforce = []
+        total_energy = []
+        for n in neb:
+            maxforce.append(n["MaxForce"])
+            total_energy.append(n["TotalEnergy"])
+
+        maxforce = np.array(maxforce)
+        total_energy = np.array(total_energy)
+
+    else:
+        print(
+            f"请检查{os.path.join(neb_dir, 'neb.h5')}或{os.path.join(neb_dir, 'neb.h5')}是否都存在！"
+        )
+
+    x = np.arange(len(maxforce))
+
+    force = maxforce
+    energy = total_energy
+
+    if raw:
+        pd.DataFrame({"x": x, "force": force, "energy": energy}).to_csv(
+            "neb_conv.csv", index=False
+        )
+
+    fig = plt.figure()
+    ax1 = fig.add_subplot(111)
+    ax1.plot(x, force, label="Max Force", c="black")
+    ax1.set_xlabel("Number of ionic step")
+    ax1.set_ylabel("Force (eV/Å)")
+    ax2 = ax1.twinx()
+    ax2.plot(x, energy, label="Energy", c="r")
+    ax2.set_xlabel("Number of ionic step")
+    ax2.set_ylabel("Energy (eV)")
+    ax2.ticklabel_format(useOffset=False)  # y轴坐标显示绝对值而不是相对值
+    fig.legend(loc=1, bbox_to_anchor=(1, 1), bbox_transform=ax1.transAxes)
+
+    plt.tight_layout()
+    # save and show
+    if figname:
+        if os.path.dirname(figname):  # not just a file name
+            os.makedirs(os.path.dirname(figname), exist_ok=True)
+        plt.savefig(figname, dpi=300)
+        print(f"--> 图片已保存为 {os.path.abspath(figname)}")
+    if show:
+        plt.show()
+
+    return ax1, ax2
+
+
+def printef(directory):
+    """打印NEB计算时各构型的能量和受力
+
+    Parameters
+    ----------
+    directory : str
+        NEB计算的目录，默认为当前目录
+
+    Returns
+    -------
+    打印各构型的能量和受力
+
+    Examples
+    --------
+    >>> from dspawpy.diffusion.nebtools import printef
+    >>> printef(directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
+        Force(eV/Å)     RC(Å)    Energy(eV)  E-E0(eV)
+    00     0.180272  0.000000 -39637.098409  0.000000
+    01     0.026337  0.542789 -39637.018595  0.079814
+    02     0.024798  1.086800 -39636.880144  0.218265
+    03     0.234429  1.588367 -39636.998366  0.100043
+    04     0.014094  2.089212 -39637.089994  0.008414
+    """
+    subfolders, resort_mfs, rcs, ens, dEs = _getef(directory)
+    data = np.array([resort_mfs, rcs, ens, dEs], dtype=float)
+    df = pd.DataFrame(
+        data.T,
+        columns=["Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
+        index=subfolders,
+    )
+    print(df)
+
+
+def restart(directory: str = ".", output: str = "bakfile"):
+    """将旧NEB任务归档压缩，并在原路径下准备续算
+
+    Parameters
+    ----------
+    directory : str
+        旧NEB任务所在路径，默认当前路径
+    output : str
+        备份文件夹路径，默认将在当前路径新建一个bakfile文件夹用于备份；
+        也可以任意指定一个路径，但不能与当前路径相同
+
+    Examples
+    ----------
+    >>> from dspawpy.diffusion.nebtools import restart
+    >>> restart(directory='/data/home/hzw1002/dspawpy_repo/test/neb_temp_back', output='/data/home/hzw1002/dspawpy_repo/test/out/neb_backup')
+    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/00压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/00.zip
+    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/01压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/01.zip
+    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/02压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/02.zip
+    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/03压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/03.zip
+    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/04压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/04.zip
+    已将/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/tmp压缩到/data/home/hzw1002/dspawpy_repo/test/out/neb_backup/neb_data.zip
+
+    续算准备工作可能需要较长时间才能完成，请耐心等待
+    """
+    while True:
+        if os.path.isdir(output):
+            if os.path.abspath(output) == os.getcwd():
+                raise ValueError("备份文件夹不能与当前路径相同！")
+            else:
+                output += "_new"
+                continue
+        else:
+            break
+
+    subfolders = get_neb_subfolders(directory, return_abs=True)  # 获取子文件夹路径
+    os.makedirs(output, exist_ok=True)  # 创建bakfile文件夹
+    # 先处理子文件夹00，01...
+    for subfolder_old in subfolders:
+        folder_index = subfolder_old.split("/")[-1]  # 00，01...
+        subfolder_back = os.path.join(output, folder_index)  # 子文件夹备份到此
+        shutil.move(subfolder_old, subfolder_back)
+        os.makedirs(subfolder_old, exist_ok=True)  # 原文件夹清空了
+
+        latestStructureFile = f"{subfolder_back}/latestStructure{folder_index}.as"
+        structureFile = f"{subfolder_back}/structure{folder_index}.as"
+
+        # 将结构文件复制到原路径下用于续算，有ls则用之，否则用s代替，都没有则报错
+        s_in_old = f"{subfolder_old}/structure{folder_index}.as"
+        if os.path.isfile(latestStructureFile):
+            shutil.copy(latestStructureFile, s_in_old)
+        elif os.path.isfile(structureFile):
+            print(f"未找到{latestStructureFile}，复用{structureFile}续算")
+            shutil.copy(structureFile, s_in_old)
+        else:
+            raise FileNotFoundError(f"{latestStructureFile}和{structureFile}都不存在！")
+
+        # 暂时放到备份主路径下，如果都没有，前面就已经报错了
+        ls_bk = os.path.join(directory, f"latestStructure{folder_index}.as")
+        s_bk = os.path.join(directory, f"structure{folder_index}.as")
+        if os.path.isfile(latestStructureFile):
+            shutil.copy(latestStructureFile, ls_bk)
+        if os.path.isfile(structureFile):
+            shutil.copy(structureFile, s_bk)
+
+        # 处理备份路径下的子文件夹
+        zf = f"{os.path.abspath(output)}/{folder_index}.zip"
+        _zip_folder(subfolder_back, zf)  # 压缩子文件夹
+        # 清空备份子文件夹
+        for file in os.listdir(subfolder_back):
+            os.remove(os.path.join(subfolder_back, file))
+
+        # 将压缩包、结构文件移入
+        shutil.move(zf, f"{subfolder_back}/{folder_index}.zip")
+        if os.path.isfile(ls_bk) and os.path.isfile(s_bk):
+            shutil.move(ls_bk, f"{subfolder_back}/latestStructure{folder_index}.as")
+            shutil.move(s_bk, f"{subfolder_back}/structure{folder_index}.as")
+        elif os.path.isfile(ls_bk):
+            shutil.move(ls_bk, f"{subfolder_back}/latestStructure{folder_index}.as")
+        elif os.path.isfile(s_bk):
+            shutil.move(s_bk, f"{subfolder_back}/structure{folder_index}.as")
+        else:
+            raise FileNotFoundError(f"{ls_bk}和{s_bk}都不存在！")
+
+    # 再处理老NEB文件夹主目录下的单个文件
+    # 备份neb.h5,neb.json和DS-PAW.log
+    tmp_dir = os.path.join(output, "tmp")
+    os.makedirs(tmp_dir, exist_ok=True)
+    if os.path.isfile(f"{directory}/neb.h5"):
+        shutil.move(f"{directory}/neb.h5", f"{tmp_dir}/neb.h5")
+    else:
+        print("未找到neb.h5，将不会备份")
+
+    if os.path.isfile(f"{directory}/neb.json"):
+        shutil.move(f"{directory}/neb.json", f"{tmp_dir}/neb.json")
+    else:
+        print("未找到neb.json，将不会备份")
+
+    if len(os.listdir(tmp_dir)) > 0:  # 如果有数据文件
+        _zip_folder(tmp_dir, f"{output}/neb_data.zip")
+        for f in os.listdir(tmp_dir):
+            os.remove(os.path.join(tmp_dir, f))
+        os.removedirs(tmp_dir)
+
+    if os.path.isfile(f"{directory}/DS-PAW.log"):
+        shutil.move(f"{directory}/DS-PAW.log", f"{output}/DS-PAW.log")
+    else:
+        print("未找到DS-PAW.log，将不会备份")
+
+
+def set_pbc(spo):
+    """根据周期性边界条件将分数坐标分量移入 [-0.5, 0.5) 区间
+
+    Parameters
+    ----------
+    spo : np.ndarray or list
+        分数坐标列表
+
+    Returns
+    -------
+    pbc_spo : np.ndarray
+        符合周期性边界条件的分数坐标列表
+
+    Examples
+    --------
+    >>> from dspawpy.diffusion.nebtools import set_pbc
+    >>> set_pbc([-0.6, 1.2, 2.3])
+    array([0.4, 0.2, 0.3])
+    """
+    # wrap into [-0.5, 0.5)
+    pbc_spo = np.mod(np.array(spo) + 0.5, 1.0) - 0.5
+
+    return pbc_spo
+
+
+def summary(
+    directory: str = ".", raw=False, show_converge=False, outdir: str = None, **kwargs
+):
+    r"""NEB任务完成总结，依次执行以下步骤：
+
+    - 1. 打印各构型受力、反应坐标、能量、与初始构型的能量差
+    - 2. 绘制能垒图
+    - 3. 绘制并保存结构优化过程的能量和受力收敛过程图
+
+    Parameters
+    ----------
+    directory : str
+        NEB路径, 默认当前路径
+    raw : bool
+        是否保存原始数据到csv文件
+    show_converge : bool
+        是否展示结构优化过程的能量和受力收敛过程图，默认不展示
+    outdir : str
+        收敛过程图保存路径，默认为directory
+    **kwargs : dict
+        传递给plot_barrier的参数
+
+    Examples
+    --------
+    >>> from dspawpy.diffusion.nebtools import summary
+    >>> directory = '/data/home/hzw1002/dspawpy_repo/test/2.15' # NEB计算路径，默认当前路径
+    >>> summary(directory, show=False)
+    --> 1. 打印NEB计算时各构型的能量和受力...
+        Force(eV/Å)     RC(Å)    Energy(eV)  E-E0(eV)
+    00     0.180272  0.000000 -39637.098409  0.000000
+    01     0.026337  0.542789 -39637.018595  0.079814
+    02     0.024798  1.086800 -39636.880144  0.218265
+    03     0.234429  1.588367 -39636.998366  0.100043
+    04     0.014094  2.089212 -39637.089994  0.008414
+    <BLANKLINE>
+    --> 2. 绘制能垒图...
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/dspaw-manual-cn/dspawpy_proj/neb_barrier.png
+    <BLANKLINE>
+    --> 3. 绘制收敛过程图到各构型文件夹中...
+    ----> /data/home/hzw1002/dspawpy_repo/test/2.15/01/converge.png...
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/2.15/01/converge.png
+    ----> /data/home/hzw1002/dspawpy_repo/test/2.15/02/converge.png...
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/2.15/02/converge.png
+    ----> /data/home/hzw1002/dspawpy_repo/test/2.15/03/converge.png...
+    --> 图片已保存为 /data/home/hzw1002/dspawpy_repo/test/2.15/03/converge.png
+    <BLANKLINE>
+    完成!
+
+    若inifin=false，用户必须将自洽的scf.h5或system.json放到初末态子文件夹中
+    """
+    # 1. 绘制能垒图
+    print("--> 1. 打印NEB计算时各构型的能量和受力...")
+    printef(directory)
+
+    # 2. 打印各构型受力、反应坐标、能量、与初始构型的能量差
+    print("\n--> 2. 绘制能垒图...")
+    plt.clf()  # 清空画布再画图
+    plot_barrier(directory=directory, raw=raw, **kwargs)
+
+    # 3. 绘制并保存结构优化过程的能量和受力收敛过程图到各构型文件夹中
+    print("\n--> 3. 绘制收敛过程图到各构型文件夹中...")
+    subfolders = get_neb_subfolders(directory)
+    for subfolder in subfolders[1 : len(subfolders) - 1]:
+        if outdir:
+            os.makedirs(os.path.join(outdir, subfolder), exist_ok=True)
+            pngfile = f"{outdir}/{subfolder}/converge.png"
+        else:
+            pngfile = f"{directory}/{subfolder}/converge.png"
+
+        print(f"----> {pngfile}...")
+        plot_neb_converge(
+            neb_dir=directory,
+            image_key=subfolder,
+            figname=pngfile,
+            raw=raw,
+            show=show_converge,
+        )
+    plt.clf()
+    print("\n完成!")
+
+
+def write_movie_json(preview: bool = False, directory: str = ".", step: int = -1):
+    r"""NEB计算或者初始插值后，读取信息，保存为 neb_movie*.json 文件
+
+    用 Device Studio 打开该文件可以观察结构等信息
+
+    Parameters
+    ----------
+    preview : bool
+        是否预览模式，默认否
+    directory : str
+        计算结果所在目录. 默认当前路径
+    step: int
+        离子步编号. 默认-1，读取整个NEB计算过程信息。
+        0表示初插结构（未完成离子步）；
+        1表示第一个离子步，以此类推。
+
+    Returns
+    ----------
+    neb_movie*.json文件
+
+    Examples
+    ----------
+    >>> from dspawpy.diffusion.nebtools import write_movie_json
+
+    NEB计算完成后要观察轨迹变化全过程，只需指定NEB计算路径即可
+
+    >>> write_movie_json(directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
+    正在读取最后一个离子步信息...
+    --> /data/home/hzw1002/dspawpy_repo/dspaw-manual-cn/dspawpy_proj/neb_movie_last.json 写入成功！
+
+    NEB计算完成后要观察第n离子步结构，请设置step为n，注意step从1开始计数
+
+    >>> write_movie_json(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', step=1)
+    正在读取第1个离子步信息...
+    --> /data/home/hzw1002/dspawpy_repo/dspaw-manual-cn/dspawpy_proj/neb_movie_1.json 写入成功！
+
+    如果您指定的step数超过NEB实际完成的离子步，将会自动修改为最后一步，实际效果等同于上一行代码
+
+    >>> write_movie_json(directory='/data/home/hzw1002/dspawpy_repo/test/2.15', step=10)
+    正在读取第10个离子步信息...
+    --> /data/home/hzw1002/dspawpy_repo/dspaw-manual-cn/dspawpy_proj/neb_movie_10.json 写入成功！
+
+    另外，如需预览初插结构，请将preview设置为True，并将directory指定为NEB计算主路径
+
+    >>> write_movie_json(preview=True, directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
+    正在根据初插结构保存neb_movie_init.json...
+    --> /data/home/hzw1002/dspawpy_repo/dspaw-manual-cn/dspawpy_proj/neb_movie_init.json 写入成功！
+    """
+
+    if preview:  # preview mode, write neb_movie_init.json from structure.as
+        print("正在根据初插结构保存neb_movie_init.json...")
+        try:
+            raw = _from_structures(directory)
+        except FileNotFoundError:
+            print("未找到初始插值结构！")
+        except Exception as e:
+            print("初始插值结构读取失败！", e)
+    else:
+        if step == 0:  # try preview mode to save time
+            try:
+                raw = _from_structures(directory)
+            except FileNotFoundError:
+                print("未找到初始插值结构，将从计算结果h5或json文件中读取！")
+            except Exception as e:
+                print("初始插值结构读取失败！", e)
+        else:
+            try:  # read from h5 file
+                raw = _from_h5(directory, step)
+            except FileNotFoundError:
+                try:  # read from json file
+                    raw = _from_json(directory, step)
+                except json.decoder.JSONDecodeError:
+                    print("json文件格式错误！")
+                except Exception as e:
+                    print(e)
+            except Exception as e:
+                print("h5文件内容读取失败！", e)
+    _dump_neb_movie_json(raw)
+
+
+def write_xyz(preview: bool = False, directory: str = ".", step: int = -1):
+    """
+    将NEB结构链条写成xyz轨迹文件用于可视化
+
+    Parameters
+    ----------
+    preview : bool
+        是否预览模式，默认否
+    directory : str
+        计算结果所在目录. 默认当前路径
+    step: int
+        离子步编号. 默认-1，读取整个NEB计算过程信息。
+        0表示初插结构（未完成离子步）；
+        1表示第一个离子步，以此类推。
+
+    Returns
+    ----------
+    neb_movie.xyz文件
+
+    Examples
+    ----------
+    >>> from dspawpy.diffusion.nebtools import write_xyz
+    >>> write_xyz(directory='/data/home/hzw1002/dspawpy_repo/test/2.15')
+    正在读取最后一个离子步信息...
+    --> /data/home/hzw1002/dspawpy_repo/dspaw-manual-cn/dspawpy_proj/neb_movie_last.xyz 写入成功！
+    <BLANKLINE>
+    """
+
+    if preview:  # preview mode, write neb_movie_init.xyz from structure.as
+        print("正在根据初插结构保存neb_movie_init.xyz...")
+        try:
+            raw = _from_structures(directory)
+        except FileNotFoundError:
+            print("未找到初始插值结构！")
+        except Exception as e:
+            print("初始插值结构读取失败！", e)
+    else:
+        if step == 0:  # try preview mode to save time
+            try:
+                raw = _from_structures(directory)
+            except FileNotFoundError:
+                print("未找到初始插值结构，将从计算结果h5或json文件中读取！")
+            except Exception as e:
+                print("初始插值结构读取失败！", e)
+        else:
+            try:  # read from h5 file
+                raw = _from_h5(directory, step)
+            except FileNotFoundError:
+                try:  # read from json file
+                    raw = _from_json(directory, step)
+                except json.decoder.JSONDecodeError:
+                    print("json文件格式错误！")
+                except Exception as e:
+                    print(e)
+            except Exception as e:
+                print("h5文件内容读取失败！", e)
+    _dump_neb_xyz(raw)
+
+
+def _dump_neb_xyz(raw):
+    """根据之前收集到的各数据列表，dump json文件到output"""
+    (
+        output,
+        subfolders,
+        step,
+        MaxForces,
+        TotalEnergies,
+        Poses,  # Nimage x Natom x 3 , read
+        Latvs,  # Nimage x 9
+        Elems,  # Nimage x Natom
+        Fixs,  # Natom x 3
+        reactionCoordinates,
+        totalEnergies,
+        maxForces,
+        tangents,
+        iDirects,
+    ) = raw
+
+    # 写入文件
+    xyzfile = output[:-5] + ".xyz"
+    Nstep = len(subfolders)  # 选定离子步，展示构型链
+    with open(xyzfile, "w") as f:
+        # Nstep
+        for n in range(Nstep):
+            eles = Elems[n]  # 针对每个构型
+            # 原子数不会变，就是不合并的元素总数
+            f.write("%d\n" % len(eles))
+            # lattice
+            f.write(
+                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
+                % (
+                    Latvs[n, 0],
+                    Latvs[n, 1],
+                    Latvs[n, 2],
+                    Latvs[n, 3],
+                    Latvs[n, 4],
+                    Latvs[n, 5],
+                    Latvs[n, 6],
+                    Latvs[n, 7],
+                    Latvs[n, 8],
+                )
+            )
+            # position and element
+            for i in range(len(eles)):
+                f.write(
+                    "%s %f %f %f\n"
+                    % (eles[i], Poses[n, i, 0], Poses[n, i, 1], Poses[n, i, 2])
+                )
+    print(f"--> {os.path.abspath(xyzfile)} 写入成功！\n")
+
+
+def _from_structures(directory: str):
+    """从structure00.as，structure01.as，...，中读取结构信息，
+    写入neb_movie_init，以便用DeviceStudio打开观察
+
+    Parameters
+    ----------
+    directory : str
+        NEB计算路径，默认当前路径
+
+    Returns
+    -------
+    用于json文件的各个数组
+    """
+    output = "neb_movie_init.json"
+    step = 0
+
+    subfolders = get_neb_subfolders(directory)
+    # print(subfolders)
+    nimage = len(subfolders)
+    reactionCoordinates = np.zeros(shape=nimage)  # optional
+    totalEnergies = np.zeros(shape=nimage)  # optional
+    maxForces = np.zeros(shape=nimage - 2)  # optional
+    tangents = np.zeros(shape=nimage - 2)  # optional
+    MaxForces = np.zeros(shape=(nimage - 2, step + 1))  # optional
+    TotalEnergies = np.zeros(shape=(nimage - 2, step + 1))  # optional
+
+    Poses = []  # nimage x Natom x 3 , read
+    Elems = []  # nimage x Natom, read
+    Latvs = []  # nimage x 9, read
+
+    iDirects = []  # read coordinate type
+    for i, folder in enumerate(subfolders):
+        structure_path = os.path.join(directory, folder, f"structure{folder}.as")
+        if not os.path.exists(structure_path):
+            raise FileNotFoundError(f"请检查{structure_path}是否存在！")
+        structure = build_Structures_from_datafile(structure_path)[0]
+        pos = structure.cart_coords
+        ele = [str(i) for i in structure.species]
+        lat = structure.lattice.matrix
+        Poses.append(pos)
+        Elems.append(ele)
+        Latvs.append(lat)
+        with open(structure_path, "r") as f:
+            lines = f.readlines()
+            coordinateType = lines[6].split()[0]
+            if coordinateType == "Direct":
+                iDirect = True
+            elif coordinateType == "Cartesian":
+                iDirect = False
+            else:
+                raise ValueError(f"请检查{structure_path}中的坐标类型！")
+            iDirects.append(iDirect)
+    Natom = len(Elems[0])
+
+    # reshape data
+    Poses = np.array(Poses).reshape((nimage, Natom, 3))
+    Elems = np.array(Elems).reshape((nimage, Natom))
+    Latvs = np.array(Latvs).reshape((nimage, 9))
+    Fixs = np.zeros(shape=(Natom, 3))  # optional
+
+    return (
+        output,
+        subfolders,
+        step,
+        MaxForces,
+        TotalEnergies,
+        Poses,
+        Latvs,
+        Elems,
+        Fixs,
+        reactionCoordinates,
+        totalEnergies,
+        maxForces,
+        tangents,
+        iDirects,
+    )
+
+
+def _from_h5(directory: str, step: int):
+    """从NEB路径下的h5文件读取 从第一步开始到指定step数 的结构和能量信息，
+    写入json文件，以便用DeviceStudio打开观察。
+
+    支持热读取结构信息（其他信息忽略）
+
+    Parameters
+    ----------
+    directory : str
+        NEB路径，默认当前路径
+    step : int
+        step数，默认-1，读取最后一个构型
+
+    Returns
+    -------
+    用于json文件的各个数组
+    """
+    # ^ 前期设置
+    neb_h5 = os.path.join(directory, "01", "neb01.h5")
+    ele = get_ele_from_h5(hpath=neb_h5)
+    Natom = len(ele)
+    data = h5py.File(neb_h5)
+    try:
+        total_steps = np.array(data.get("/NebSize"))[0]
+    except:
+        print("NEB计算未正常结束，正在尝试实时读取结构信息...")
+        try:
+            total_steps = np.array(data.get("/Structures/FinalStep"))[0]
+        except:
+            raise ValueError("尚未完成第一个离子步，请检查计算是否出错，否则请耐心等待离子步完成至少一个后再尝试读取！")
+
+    if step == -1:
+        output = "neb_movie_last.json"
+        step = total_steps
+        print("正在读取最后一个离子步信息...")
+    elif step > total_steps:
+        output = "neb_movie_last.json"
+        step = total_steps
+        print(f"指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
+        print("正在读取最后一个离子步信息...")
+    else:
+        output = "neb_movie_{}.json".format(step)
+        print(f"正在读取第{step}个离子步信息...")
+
+    # ^ 读取前，准备好json文件所需数组框架
+    subfolders = get_neb_subfolders(directory)
+    nimage = len(subfolders)
+    reactionCoordinates = np.zeros(shape=nimage)  # optional
+    totalEnergies = np.zeros(shape=nimage)  # optional，每个构型最终能量
+    maxForces = np.zeros(shape=nimage - 2)  # optional
+    tangents = np.zeros(shape=nimage - 2)  # optional
+    MaxForces = np.zeros(shape=(nimage - 2, step))  # optional
+    TotalEnergies = np.zeros(shape=(nimage - 2, step))  # optional，中间构型每个离子步能量
+    # Sposes = []  # nimage x Natom x 3 , read
+    Sposes = np.empty(shape=(nimage, Natom, 3))  # nimage x Natom x 3 , read
+    Elems = []  # nimage x Natom, read
+    Latvs = []  # nimage x 9, read
+    Fixs = []  # Natom x 3, set
+
+    for folder in subfolders:
+        """如果是首尾两个构型，最多只有scf.h5文件，没有neb.h5文件
+        用户如果算NEB的时候，不计算首尾构型的自洽，
+         或者在别处算完了但是没有复制到首尾文件夹中并命名为scf.h5，
+          便不能使用第一个功能
+        """
+        if folder == subfolders[0] or folder == subfolders[-1]:
+            h5_path = os.path.join(directory, folder, "scf.h5")
+            spath = os.path.join(directory, folder, f"structure{folder}.as")
+            assert os.path.exists(h5_path) or os.path.exists(
+                spath
+            ), f"请确认{h5_path}或{spath}至少存在一个！"
+        else:
+            h5_path = os.path.join(directory, folder, f"neb{folder}.h5")
+            assert os.path.exists(h5_path), f"请确认{h5_path}是否存在！"
+
+    # ^ 开始分功能读取数据
+    for i, folder in enumerate(subfolders):
+        if folder == subfolders[0] or folder == subfolders[-1]:
+            h5_path = os.path.join(directory, folder, "scf.h5")
+            if os.path.exists(h5_path):
+                data = h5py.File(h5_path)
+                # 不影响可视化，直接定为0
+                if folder == subfolders[0]:
+                    reactionCoordinates[i] = 0
+                pos = np.array(data.get("/Structures/Step-1/Position")).reshape(
+                    -1, 3
+                )  # scaled
+                lat = np.array(data.get("/Structures/Step-1/Lattice"))
+                ele = get_ele_from_h5(hpath=h5_path)
+                totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
+            else:
+                structure = build_Structures_from_datafile(spath)[0]
+                pos = structure.frac_coords
+                ele = [str(i) for i in structure.species]
+                lat = structure.lattice.matrix
+        else:
+            h5_path = os.path.join(directory, folder, f"neb{folder}.h5")
+            data = h5py.File(h5_path)
+            # reading...
+            try:
+                reactionCoordinates[i - 1] = np.array(data.get("/Distance/Previous"))[
+                    -1
+                ]
+                maxForces[i - 1] = np.array(data.get("/MaxForce"))[-1]
+                tangents[i - 1] = np.array(data.get("/Tangent"))[-1]
+                if folder == subfolders[-2]:
+                    reactionCoordinates[i + 1] = np.array(data.get("/Distance/Next"))[
+                        -1
+                    ]
+                # read MaxForces and TotalEnergies
+                nionStep = np.array(data.get("/MaxForce")).shape[0]
+                assert step <= nionStep, f"总共只完成了{nionStep}个离子步!"
+                for j in range(step):
+                    MaxForces[i - 1, j] = np.array(data.get("/MaxForce"))[j]
+                    TotalEnergies[i - 1, j] = np.array(data.get("/TotalEnergy"))[j]
+                totalEnergies[i] = np.array(data.get("/Energy/TotalEnergy0"))
+            except:
+                pass  # 还没完成NEB计算，不影响读取结构信息用于可视化
+            # read the latest structure for visualization
+            pos = np.array(data.get(f"/Structures/Step-{step}/Position")).reshape(
+                Natom, 3
+            )  # scaled
+            lat = np.array(data.get(f"/Structures/Step-{step}/Lattice"))
+            ele = get_ele_from_h5(hpath=h5_path)
+
+        Elems.append(ele)
+        Sposes[i, :, :] = pos
+        Latvs.append(lat)
+
+    if os.path.exists(os.path.join(directory, "neb.h5")):
+        tdata = h5py.File(os.path.join(directory, "neb.h5"))
+        # atom fix, not lattice
+        # ignore this trivial message because it is not necessary for the visualization
+        if "/UnrelaxStructure/Image00/Fix" in tdata:
+            fix_array = np.array(tdata.get("/UnrelaxStructure/Image00/Fix"))
+            for fix in fix_array:
+                if fix == 0.0:
+                    F = False
+                elif fix == 1.0:
+                    F = True
+                else:
+                    raise ValueError("Fix值只能为0或1")
+                Fixs.append(F)
+        else:
+            Fixs = np.full(shape=(Natom, 3), fill_value=False)
+    else:
+        Fixs = np.full(shape=(Natom, 3), fill_value=False)
+
+    Elems = np.array(Elems).reshape((nimage, Natom))
+    Latvs = np.array(Latvs).reshape((nimage, 9))
+    Fixs = np.array(Fixs).reshape((Natom, 3))
+    iDirects = [True for i in range(Natom)]  # only output direct coordinates
+
+    return (
+        output,
+        subfolders,
+        step,
+        MaxForces,
+        TotalEnergies,  #
+        Sposes,
+        Latvs,
+        Elems,
+        Fixs,
+        reactionCoordinates,
+        totalEnergies,
+        maxForces,
+        tangents,
+        iDirects,
+    )
+
+
+def _from_json(directory: str, step: int):
+    """从NEB路径下的json文件读取 从第一步开始到指定step数 的结构和能量信息，
+    写入json文件，以便用DeviceStudio打开观察
+
+    Parameters
+    ----------
+    directory : str
+        NEB路径，默认当前路径
+    step : int
+        step数，默认-1，读取最后一个构型
+
+    Returns
+    -------
+    用于json文件的各个数组
+    """
+
+    # ^ 前期设置
+    neb_js = os.path.join(directory, "01/neb01.json")
+    with open(neb_js, "r") as f:
+        data = json.load(f)
+    total_steps = len(data)
+
+    if step == -1:
+        output = "neb_movie_last.json"
+        step = total_steps
+        print("正在读取最后一个离子步信息（h5文件不存在，尝试从json文件读取数据）...")
+    elif step > total_steps:
+        output = "neb_movie_last.json"
+        step = total_steps
+        print(f"您指定的step数大于NEB计算实际完成的总离子步数{total_steps}")
+        print("正在读取最后一个离子步信息（h5文件不存在，尝试从json文件读取数据）...")
+    else:
+        output = f"neb_movie_{step}.json"
+        print(f"正在读取第{step}个离子步信息...")
+
+    # ^ 读取前，准备好json文件所需数组框架
+    subfolders = get_neb_subfolders(directory)
+    nimage = len(subfolders)
+    reactionCoordinates = np.zeros(shape=nimage)  # optional
+    totalEnergies = np.zeros(shape=nimage)  # optional，每个构型最终能量
+    maxForces = np.zeros(shape=nimage - 2)  # optional
+    tangents = np.zeros(shape=nimage - 2)  # optional
+    MaxForces = np.zeros(shape=(nimage - 2, step))  # optional
+    TotalEnergies = np.zeros(shape=(nimage - 2, step))  # optional，中间构型每个离子步能量
+    Sposes = []  # nimage x Natom x 3 , read
+    Elems = []  # nimage x Natom, read
+    Latvs = []  # nimage x 9, read
+    Fixs = []  # Natom x 3, set
+
+    for folder in subfolders:
+        """如果是首尾两个构型，最多只有system.json文件，没有neb*.json文件
+        用户如果算NEB的时候，不计算首尾构型的自洽，
+         或者在别处算完了但是没有复制到首尾文件夹中并命名为system.json，
+          便不能使用第一个功能
+        """
+        if folder == subfolders[0] or folder == subfolders[-1]:
+            js_path = os.path.join(directory, folder, "system.json")
+        else:
+            js_path = os.path.join(directory, folder, f"neb{folder}.json")
+        assert os.path.exists(js_path), f"请确认{js_path}是否存在！"
+
+    # ^ 开始分功能读取数据
+    for i, folder in enumerate(subfolders):
+        if i == 0:  # 初末态在NEB计算过程中不会优化结构
+            # 1. 外部自洽后移动system.json
+            js_path = os.path.join(directory, folder, "system.json")
+            # 2. 直接NEB计算，得到system00.json
+            neb_js_path = os.path.join(directory, folder, f"system{folder}.json")
+            if os.path.exists(neb_js_path):  # 优先读取neb计算得到的system00.json
+                with open(neb_js_path, "r") as f:
+                    data = json.load(f)
+
+            elif os.path.exists(js_path):
+                with open(js_path, "r") as f:
+                    data = json.load(f)
+
+            else:
+                raise FileNotFoundError(
+                    f"{os.path.abspath(js_path)}和{os.path.abspath(neb_js_path)}均不存在！"
+                )
+
+            lat = data["AtomInfo"]["Lattice"]
+            Latvs.append(lat)
+
+            Natom = len(data["AtomInfo"]["Atoms"])  # 读取原子数
+            for j in range(Natom):
+                pos = data["AtomInfo"]["Atoms"][j]["Position"]  # scaled
+                Sposes.append(pos)
+
+            totalEnergies[i] = data["Energy"]["TotalEnergy0"]
+            reactionCoordinates[i] = 0.0
+
+        elif i > 0 and i < nimage - 1:  # 中间构型会优化结构
+            # 读取晶胞矢量、原子坐标
+            relax_json = os.path.join(directory, folder, "relax.json")
+            assert os.path.exists(relax_json), f"{relax_json}不存在！"
+
+            with open(relax_json, "r") as f:
+                rdata = json.load(f)
+
+            lat = rdata[step - 1]["Lattice"]  # 第step步优化后的晶胞
+            Latvs.append(lat)
+
+            Natom = len(rdata[0]["Atoms"])
+            for j in range(Natom):  # for each atom
+                pos = rdata[step - 1]["Atoms"][j]["Position"]  # 第step步优化后的原子坐标
+                Sposes.append(pos)  # ! 输出的都是分数坐标
+
+            # 读取能量和反应坐标
+            nj = os.path.join(directory, folder, f"neb{folder}.json")
+            with open(nj, "r") as f:
+                print(f"Reading {os.path.abspath(nj)}...")
+                ndata = json.load(f)
+
+            totalEnergies[i] = ndata[step - 1]["TotalEnergy"]  # 读取第step步优化后的能量
+
+            # 读取与前一个构型相比的反应坐标
+            reactionCoordinates[i - 1] = ndata[step - 1]["ReactionCoordinate"][-2]
+            tangents[i - 1] = ndata[step - 1]["Tangent"]
+            if folder == subfolders[-2]:  # 末态前一个构型的计算结果中读取反应坐标
+                reactionCoordinates[i + 1] = ndata[step - 1]["ReactionCoordinate"][-1]
+            for j in range(step):
+                MaxForces[i - 1, j] = ndata[j]["MaxForce"]
+                # neb01.json中不存在TotalEnergy0，暂时读取TotalEnergy
+                TotalEnergies[i - 1, j] = ndata[j]["TotalEnergy"]
+
+        else:  # 末态构型
+            js_path = os.path.join(directory, folder, "system.json")
+            neb_js_path = os.path.join(directory, folder, f"system{folder}.json")
+            if os.path.exists(neb_js_path):  # 优先读取neb计算得到的json文件
+                with open(neb_js_path, "r") as f:
+                    data = json.load(f)
+
+            elif os.path.exists(js_path):
+                with open(js_path, "r") as f:
+                    data = json.load(f)
+
+            else:
+                raise FileNotFoundError(
+                    f"{os.path.abspath(js_path)}和{os.path.abspath(neb_js_path)}均不存在！"
+                )
+
+            lat = data["AtomInfo"]["Lattice"]
+            Latvs.append(lat)
+
+            Natom = len(data["AtomInfo"]["Atoms"])  # 读取原子数
+            for j in range(Natom):
+                pos = data["AtomInfo"]["Atoms"][j]["Position"]  # scaled
+                Sposes.append(pos)
+
+            energy = data["Energy"]["TotalEnergy0"]
+            totalEnergies[i] = energy
+
+    # 读取原子元素
+    tneb_js = os.path.join(directory, "neb.json")
+    with open(tneb_js, "r") as f:
+        tdata = json.load(f)
+
+    Natom = len(tdata["UnrelaxStructure"][0]["Atoms"])
+    elems = []
+    for k in range(Natom):
+        ele = tdata["UnrelaxStructure"][0]["Atoms"][k]["Element"]
+        elems.append(ele)
+
+    for ni in range(nimage):
+        Elems.append(elems)  # 重复nimage次，保持Elems结构一致
+
+    for atom in range(Natom):
+        fix_array = tdata["UnrelaxStructure"][1]["Atoms"][atom]["Fix"]  # (1,3)
+        if fix_array == []:  # empty list
+            fix_array = [0.0, 0.0, 0.0]
+        for fix in fix_array:
+            if fix == 0.0:
+                F = False
+            elif fix == 1.0:
+                F = True
+            else:
+                raise ValueError("Fix值只能为 0.0 或 1.0")
+            Fixs.append(F)
+
+    # 累加reactionCoordinates中的元素
+    for i in range(1, len(reactionCoordinates)):
+        reactionCoordinates[i] += reactionCoordinates[i - 1]
+
+    # reshape data
+    Sposes = np.array(Sposes).reshape((nimage, Natom, 3))
+    Elems = np.array(Elems).reshape((nimage, Natom))
+    Latvs = np.array(Latvs).reshape((nimage, 9))
+    Fixs = np.array(Fixs).reshape((Natom, 3))
+    iDirects = [True for i in range(Natom)]  # only output direct coordinates
+
+    return (
+        output,
+        subfolders,
+        step,
+        MaxForces,
+        TotalEnergies,
+        Sposes,
+        Latvs,
+        Elems,
+        Fixs,
+        reactionCoordinates,
+        totalEnergies,
+        maxForces,
+        tangents,
+        iDirects,
+    )
+
+
+def _dump_neb_movie_json(raw):
+    """根据之前收集到的各数据列表，dump json文件到output"""
+    (
+        output,
+        subfolders,
+        step,
+        MaxForces,
+        TotalEnergies,
+        Poses,
+        Latvs,
+        Elems,
+        Fixs,
+        reactionCoordinates,
+        totalEnergies,
+        maxForces,
+        tangents,
+        iDirects,
+    ) = raw
+
+    IterDict = {}
+    for s, sf in enumerate(subfolders):
+        if sf == subfolders[0] or sf == subfolders[-1]:
+            continue
+        else:
+            Eflist = []
+            for l in range(step):
+                ef = {
+                    "MaxForce": MaxForces[s - 1, l],
+                    "TotalEnergy": TotalEnergies[s - 1, l],
+                }
+                Eflist.append(ef)
+                iterDict = {sf: Eflist}  # construct sub-dict
+                IterDict.update(iterDict)  # append sub-dict
+
+    RSList = []
+    """
+    从外到内依次遍历 构型、原子（子字典）
+    原子的键值对为：'Atoms': 原子信息列表
+    原子信息列表是一个由字典组成的列表，每个字典对应一个原子的信息
+    """
+    for s, sf in enumerate(subfolders):
+        pos = Poses[s]
+        lat = Latvs[s]
+        elem = Elems[s]
+        atoms = []
+        for i in range(len(elem)):
+            atom = {
+                "Element": elem[i],
+                "Fix": Fixs[i].tolist(),
+                "Mag": [],  # empty
+                "Position": pos[i].tolist(),
+                "Pot": "",
+            }  # empty
+            atoms.append(atom)
+        if iDirects[s]:
+            rs = {"Atoms": atoms, "CoordinateType": "Direct", "Lattice": lat.tolist()}
+        else:
+            rs = {
+                "Atoms": atoms,
+                "CoordinateType": "Cartesian",
+                "Lattice": lat.tolist(),
+            }
+        RSList.append(rs)
+
+    URSList = []  # DS似乎并不读取这部分信息，空置即可
+
+    data = {
+        "Distance": {"ReactionCoordinate": reactionCoordinates.tolist()},
+        "Energy": {"TotalEnergy": totalEnergies.tolist()},
+        "Force": {"MaxForce": maxForces.tolist(), "Tangent": tangents.tolist()},
+        "Iteration": IterDict,
+        "RelaxedStructure": RSList,
+        "UnrelaxedStructure": URSList,
+    }
+
+    # ^ 将字典写入json文件
+    with open(output, "w") as f:
+        json.dump(data, f, indent=4)
+
+    print(f"--> {os.path.abspath(output)} 写入成功！")
+
+
+def _getef(directory: str = "."):
+    """读取NEB计算时各构型的能量和受力，NEB计算可以未收敛
+    但如果初末态自洽在别处完成，请手动将其移入00等文件夹中！
+
+    Parameters
+    ----------
+    directory: str
+        NEB计算的路径，默认当前路径
+
+    Returns
+    -------
+    subfolders: list
+        构型文件夹名列表
+    resort_mfs: list
+        构型受力的最大分量列表
+    rcs: list
+        反应坐标列表
+    ens: list
+        电子总能列表
+    dEs: list
+        与初始构型的能量差列表
+    """
+
+    subfolders = get_neb_subfolders(directory)
+    Nimage = len(subfolders)
+
+    ens = []
+    dEs = np.zeros(Nimage)
+    rcs = [0]
+    mfs = []
+
+    # read energies
+    count = 1
+    for i, subfolder in enumerate(subfolders):
+        if i == 0 or i == Nimage - 1:
+            jsf = os.path.join(directory, subfolder, f"system{subfolder}.json")
+            old_jsf = os.path.join(directory, subfolder, "system.json")
+            hf = os.path.join(directory, subfolder, "scf.h5")
+
+            if os.path.exists(hf):  # 优先读取h5文件内容
+                data = h5py.File(hf)
+                en = np.array(data.get("/Energy/TotalEnergy0"))[0]
+                if i == 0 or i == Nimage - 1:
+                    mf = np.max(np.abs(np.array(data.get("/Force/ForceOnAtoms"))))
+                    mfs.append(mf)
+
+            elif os.path.exists(jsf):  # 其次读取json文件内容
+                with open(jsf, "r") as f:
+                    data = json.load(f)
+                en = data["Energy"]["TotalEnergy0"]
+                if i == 0 or i == Nimage - 1:
+                    mf = np.max(np.abs(data["Force"]["ForceOnAtoms"]))
+                    mfs.append(mf)
+
+            elif os.path.exists(old_jsf):  # 兼容老json
+                with open(old_jsf, "r") as f:
+                    data = json.load(f)
+                en = data["Energy"]["TotalEnergy0"]
+                if i == 0 or i == Nimage - 1:
+                    mf = np.max(np.abs(data["Force"]["ForceOnAtoms"]))
+                    mfs.append(mf)
+
+            else:
+                raise FileNotFoundError(
+                    "无法找到记录构型%s的能量和受力的system.json或scf.h5文件" % subfolder
+                )
+            ens.append(en)
+
+        else:
+            jsf = os.path.join(directory, subfolder, f"neb{subfolder}.json")
+            sysjsf = os.path.join(directory, subfolder, f"system{subfolder}.json")
+            old_sysjsf = os.path.join(directory, subfolder, "system.json")
+            hf = os.path.join(directory, subfolder, f"neb{subfolder}.h5")
+
+            if os.path.exists(hf):  # 优先读取h5文件内容
+                data = h5py.File(hf)
+                en = np.array(data.get("/Energy/TotalEnergy0"))[0]
+                mf = np.array(data.get("/MaxForce"))[-1]
+                # the key may change depends on your DS-PAW version
+                if "/Distance/Previous" in data:
+                    rc = np.array(data.get("/Distance/Previous"))[-1]
+                elif "/ReactionCoordinate" in data:
+                    rc = np.array(data.get("/ReactionCoordinate"))[-2]
+                else:
+                    raise KeyError("找不到/Distance/Previous或/ReactionCoordinate键！")
+                rcs.append(rc)
+                if count == Nimage - 2:  # before final image
+                    if "/Distance/Next" in data:
+                        rc = np.array(data.get("/Distance/Next"))[-1]
+                    elif "/ReactionCoordinate" in data:
+                        rc = np.array(data.get("/ReactionCoordinate"))[-1]
+                    else:
+                        raise KeyError("找不到/Distance/Next或/ReactionCoordinate键！")
+                    rcs.append(rc)
+
+            elif os.path.exists(jsf):
+                if os.path.exists(sysjsf):
+                    with open(sysjsf, "r") as f:
+                        data = json.load(f)
+                    en = data["Energy"]["TotalEnergy0"]
+                elif os.path.exists(old_sysjsf):  # 兼容旧版DS-PAW
+                    with open(old_sysjsf, "r") as f:
+                        data = json.load(f)
+                    en = data["Energy"]["TotalEnergy0"]
+                else:
+                    raise FileNotFoundError(f"无法找到{sysjsf}或{old_sysjsf}")
+
+                with open(jsf, "r") as f:
+                    data = json.load(f)
+                Nion_step = len(data)
+                # en = data[Nion_step - 1]["TotalEnergy"] # invalid
+                mf = data[Nion_step - 1]["MaxForce"]  # 最后一步的最大受力
+                rc = data[Nion_step - 1]["ReactionCoordinate"][0]  # 最后一步的反应坐标
+                rcs.append(rc)
+                if count == Nimage - 2:  # before final image
+                    rc = data[Nion_step - 1]["ReactionCoordinate"][1]  # 最后一步的反应坐标
+                    rcs.append(rc)
+
+            else:
+                raise FileNotFoundError(f"无法找到{hf}或{jsf}")
+
+            ens.append(en)
+            mfs.append(mf)
+
+            # get dE
+            dE = ens[count] - ens[0]
+            dEs[i] = dE
+            count += 1
+    dEs[-1] = ens[Nimage - 1] - ens[0]
+
+    # rcs 改成累加值
+    for i in range(1, len(rcs)):
+        rcs[i] += rcs[i - 1]
+
+    rcs = np.array(rcs)
+
+    resort_mfs = [mfs[0]]
+    final_mf = mfs[1]
+    for j in range(2, len(mfs)):
+        resort_mfs.append(mfs[j])
+    resort_mfs.append(final_mf)
+
+    return subfolders, resort_mfs, rcs, ens, dEs
```

## dspawpy/diffusion/pathfinder.py

 * *Ordering differences only*

```diff
@@ -1,287 +1,287 @@
-# -*- coding: utf-8 -*-
-import itertools
-import warnings
-
-import numpy as np
-from pymatgen.core import PeriodicSite, Structure
-from pymatgen.core.periodic_table import get_el_sp
-
-
-# copy from pymatgen-analysis-diffusion https://github.com/materialsvirtuallab/pymatgen-analysis-diffusion
-class IDPPSolver:
-    """
-    A solver using image dependent pair potential (IDPP) algo to get an improved
-    initial NEB path. For more details about this algo, please refer to
-    Smidstrup et al., J. Chem. Phys. 140, 214106 (2014).
-
-    """
-
-    def __init__(self, structures):
-        """
-        Initialization.
-
-        Args:
-            structures (list of pmg_structure) : Initial guess of the NEB path
-                (including initial and final end-point structures).
-        """
-
-        latt = structures[0].lattice
-        natoms = structures[0].num_sites
-        nimages = len(structures) - 2
-        target_dists = []
-
-        # Initial guess of the path (in Cartesian coordinates) used in the IDPP
-        # algo.
-        init_coords = []
-
-        # Construct the set of target distance matrices via linear interpolation
-        # between those of end-point structures.
-        for i in range(1, nimages + 1):
-            # Interpolated distance matrices
-            dist = structures[0].distance_matrix + i / (nimages + 1) * (
-                structures[-1].distance_matrix - structures[0].distance_matrix
-            )
-
-            target_dists.append(dist)
-
-        target_dists = np.array(target_dists)
-
-        # Set of translational vector matrices (anti-symmetric) for the images.
-        translations = np.zeros((nimages, natoms, natoms, 3), dtype=np.float64)
-
-        # A set of weight functions. It is set as 1/d^4 for each image. Here,
-        # we take d as the average of the target distance matrix and the actual
-        # distance matrix.
-        weights = np.zeros_like(target_dists, dtype=np.float64)
-        for ni in range(nimages):
-            avg_dist = (target_dists[ni] + structures[ni + 1].distance_matrix) / 2.0
-            weights[ni] = 1.0 / (
-                avg_dist**4 + np.eye(natoms, dtype=np.float64) * 1e-8
-            )
-
-        for ni, i in itertools.product(range(nimages + 2), range(natoms)):
-            frac_coords = structures[ni][i].frac_coords
-            init_coords.append(latt.get_cartesian_coords(frac_coords))
-
-            if ni not in [0, nimages + 1]:
-                for j in range(i + 1, natoms):
-                    img = latt.get_distance_and_image(
-                        frac_coords, structures[ni][j].frac_coords
-                    )[1]
-                    translations[ni - 1, i, j] = latt.get_cartesian_coords(img)
-                    translations[ni - 1, j, i] = -latt.get_cartesian_coords(img)
-
-        self.init_coords = np.array(init_coords).reshape(nimages + 2, natoms, 3)
-        self.translations = translations
-        self.weights = weights
-        self.structures = structures
-        self.target_dists = target_dists
-        self.nimages = nimages
-
-    def run(
-        self,
-        maxiter=1000,
-        tol=1e-5,
-        gtol=1e-3,
-        step_size=0.05,
-        max_disp=0.05,
-        spring_const=5.0,
-        species=None,
-    ):
-        """
-        Perform iterative minimization of the set of objective functions in an
-        NEB-like manner. In each iteration, the total force matrix for each
-        image is constructed, which comprises both the spring forces and true
-        forces. For more details about the NEB approach, please see the
-        references, e.g. Henkelman et al., J. Chem. Phys. 113, 9901 (2000).
-
-        Args:
-            maxiter (int): Maximum number of iterations in the minimization
-                process.
-            tol (float): Tolerance of the change of objective functions between
-                consecutive steps.
-            gtol (float): Tolerance of maximum force component (absolute value).
-            step_size (float): Step size associated with the displacement of
-                the atoms during the minimization process.
-            max_disp (float): Maximum allowed atomic displacement in each
-                iteration.
-            spring_const (float): A virtual spring constant used in the NEB-like
-                        relaxation process that yields so-called IDPP path.
-            species (list of string): If provided, only those given species are
-                allowed to move. The atomic positions of other species are
-                obtained via regular linear interpolation approach.
-
-        Returns:
-            [Structure] Complete IDPP path (including end-point structures)
-        """
-
-        coords = self.init_coords.copy()
-        old_funcs = np.zeros((self.nimages,), dtype=np.float64)
-        idpp_structures = [self.structures[0]]
-
-        if species is None:
-            indices = list(range(len(self.structures[0])))
-        else:
-            species = [get_el_sp(sp) for sp in species]
-            indices = [
-                i for i, site in enumerate(self.structures[0]) if site.specie in species
-            ]
-
-            if len(indices) == 0:
-                raise ValueError("The given species are not in the system!")
-
-        # Iterative minimization
-        for n in range(maxiter):
-            # Get the sets of objective functions, true and total force
-            # matrices.
-            funcs, true_forces = self._get_funcs_and_forces(coords)
-            tot_forces = self._get_total_forces(
-                coords, true_forces, spring_const=spring_const
-            )
-
-            # Each atom is allowed to move up to max_disp
-            disp_mat = step_size * tot_forces[:, indices, :]
-            disp_mat = np.where(
-                np.abs(disp_mat) > max_disp, np.sign(disp_mat) * max_disp, disp_mat
-            )
-            coords[1 : (self.nimages + 1), indices] += disp_mat
-
-            max_force = np.abs(tot_forces[:, indices, :]).max()
-            tot_res = np.sum(np.abs(old_funcs - funcs))
-
-            if tot_res < tol and max_force < gtol:
-                break
-
-            old_funcs = funcs
-
-        else:
-            warnings.warn(
-                "Maximum iteration number is reached without convergence!", UserWarning
-            )
-
-        for ni in range(self.nimages):
-            # generate the improved image structure
-            new_sites = []
-
-            for site, cart_coords in zip(self.structures[ni + 1], coords[ni + 1]):
-                new_site = PeriodicSite(
-                    site.species,
-                    coords=cart_coords,
-                    lattice=site.lattice,
-                    coords_are_cartesian=True,
-                    properties=site.properties,
-                )
-                new_sites.append(new_site)
-
-            idpp_structures.append(Structure.from_sites(new_sites))
-
-        # Also include end-point structure.
-        idpp_structures.append(self.structures[-1])
-
-        return idpp_structures
-
-    @classmethod
-    def from_endpoints(cls, endpoints, nimages=5, sort_tol=1.0):
-        """
-        A class method that starts with end-point structures instead. The
-        initial guess for the IDPP algo is then constructed using linear
-        interpolation.
-
-        Args:
-            endpoints (list of Structure objects): The two end-point structures.
-            nimages (int): Number of images between the two end-points.
-            sort_tol (float): Distance tolerance (in Angstrom) used to match the
-                atomic indices between start and end structures. Need
-                to increase the value in some cases.
-        """
-        try:
-            images = endpoints[0].interpolate(
-                endpoints[1],
-                nimages=nimages + 1,
-                interpolate_lattices=True,
-                autosort_tol=sort_tol,
-            )
-        except Exception as e:
-            if "Unable to reliably match structures " in str(e):
-                warnings.warn(
-                    "Auto sorting is turned off because it is unable"
-                    " to match the end-point structures!",
-                    UserWarning,
-                )
-                images = endpoints[0].interpolate(
-                    endpoints[1], nimages=nimages + 1, autosort_tol=0
-                )
-            else:
-                raise e
-
-        return IDPPSolver(images)
-
-    def _get_funcs_and_forces(self, x):
-        """
-        Calculate the set of objective functions as well as their gradients,
-        i.e. "effective true forces"
-        """
-        funcs = []
-        funcs_prime = []
-        trans = self.translations
-        natoms = trans.shape[1]
-        weights = self.weights
-        target_dists = self.target_dists
-
-        for ni in range(len(x) - 2):
-            vec = [x[ni + 1, i] - x[ni + 1] - trans[ni, i] for i in range(natoms)]
-
-            trial_dist = np.linalg.norm(vec, axis=2)
-            aux = (
-                (trial_dist - target_dists[ni])
-                * weights[ni]
-                / (trial_dist + np.eye(natoms, dtype=np.float64))
-            )
-
-            # Objective function
-            func = np.sum((trial_dist - target_dists[ni]) ** 2 * weights[ni])
-
-            # "True force" derived from the objective function.
-            grad = np.sum(aux[:, :, None] * vec, axis=1)
-
-            funcs.append(func)
-            funcs_prime.append(grad)
-
-        return 0.5 * np.array(funcs), -2 * np.array(funcs_prime)
-
-    @staticmethod
-    def get_unit_vector(vec):
-        return vec / np.sqrt(np.sum(vec**2))
-
-    def _get_total_forces(self, x, true_forces, spring_const):
-        """
-        Calculate the total force on each image structure, which is equal to
-        the spring force along the tangent + true force perpendicular to the
-        tangent. Note that the spring force is the modified version in the
-        literature (e.g. Henkelman et al., J. Chem. Phys. 113, 9901 (2000)).
-        """
-
-        total_forces = []
-        natoms = np.shape(true_forces)[1]
-
-        for ni in range(1, len(x) - 1):
-            vec1 = (x[ni + 1] - x[ni]).flatten()
-            vec2 = (x[ni] - x[ni - 1]).flatten()
-
-            # Local tangent
-            tangent = self.get_unit_vector(vec1) + self.get_unit_vector(vec2)
-            tangent = self.get_unit_vector(tangent)
-
-            # Spring force
-            spring_force = (
-                spring_const * (np.linalg.norm(vec1) - np.linalg.norm(vec2)) * tangent
-            )
-
-            # Total force
-            flat_ft = true_forces[ni - 1].copy().flatten()
-            total_force = true_forces[ni - 1] + (
-                spring_force - np.dot(flat_ft, tangent) * tangent
-            ).reshape(natoms, 3)
-            total_forces.append(total_force)
-
-        return np.array(total_forces)
+# -*- coding: utf-8 -*-
+import itertools
+import warnings
+
+import numpy as np
+from pymatgen.core import PeriodicSite, Structure
+from pymatgen.core.periodic_table import get_el_sp
+
+
+# copy from pymatgen-analysis-diffusion https://github.com/materialsvirtuallab/pymatgen-analysis-diffusion
+class IDPPSolver:
+    """
+    A solver using image dependent pair potential (IDPP) algo to get an improved
+    initial NEB path. For more details about this algo, please refer to
+    Smidstrup et al., J. Chem. Phys. 140, 214106 (2014).
+
+    """
+
+    def __init__(self, structures):
+        """
+        Initialization.
+
+        Args:
+            structures (list of pmg_structure) : Initial guess of the NEB path
+                (including initial and final end-point structures).
+        """
+
+        latt = structures[0].lattice
+        natoms = structures[0].num_sites
+        nimages = len(structures) - 2
+        target_dists = []
+
+        # Initial guess of the path (in Cartesian coordinates) used in the IDPP
+        # algo.
+        init_coords = []
+
+        # Construct the set of target distance matrices via linear interpolation
+        # between those of end-point structures.
+        for i in range(1, nimages + 1):
+            # Interpolated distance matrices
+            dist = structures[0].distance_matrix + i / (nimages + 1) * (
+                structures[-1].distance_matrix - structures[0].distance_matrix
+            )
+
+            target_dists.append(dist)
+
+        target_dists = np.array(target_dists)
+
+        # Set of translational vector matrices (anti-symmetric) for the images.
+        translations = np.zeros((nimages, natoms, natoms, 3), dtype=np.float64)
+
+        # A set of weight functions. It is set as 1/d^4 for each image. Here,
+        # we take d as the average of the target distance matrix and the actual
+        # distance matrix.
+        weights = np.zeros_like(target_dists, dtype=np.float64)
+        for ni in range(nimages):
+            avg_dist = (target_dists[ni] + structures[ni + 1].distance_matrix) / 2.0
+            weights[ni] = 1.0 / (
+                avg_dist**4 + np.eye(natoms, dtype=np.float64) * 1e-8
+            )
+
+        for ni, i in itertools.product(range(nimages + 2), range(natoms)):
+            frac_coords = structures[ni][i].frac_coords
+            init_coords.append(latt.get_cartesian_coords(frac_coords))
+
+            if ni not in [0, nimages + 1]:
+                for j in range(i + 1, natoms):
+                    img = latt.get_distance_and_image(
+                        frac_coords, structures[ni][j].frac_coords
+                    )[1]
+                    translations[ni - 1, i, j] = latt.get_cartesian_coords(img)
+                    translations[ni - 1, j, i] = -latt.get_cartesian_coords(img)
+
+        self.init_coords = np.array(init_coords).reshape(nimages + 2, natoms, 3)
+        self.translations = translations
+        self.weights = weights
+        self.structures = structures
+        self.target_dists = target_dists
+        self.nimages = nimages
+
+    def run(
+        self,
+        maxiter=1000,
+        tol=1e-5,
+        gtol=1e-3,
+        step_size=0.05,
+        max_disp=0.05,
+        spring_const=5.0,
+        species=None,
+    ):
+        """
+        Perform iterative minimization of the set of objective functions in an
+        NEB-like manner. In each iteration, the total force matrix for each
+        image is constructed, which comprises both the spring forces and true
+        forces. For more details about the NEB approach, please see the
+        references, e.g. Henkelman et al., J. Chem. Phys. 113, 9901 (2000).
+
+        Args:
+            maxiter (int): Maximum number of iterations in the minimization
+                process.
+            tol (float): Tolerance of the change of objective functions between
+                consecutive steps.
+            gtol (float): Tolerance of maximum force component (absolute value).
+            step_size (float): Step size associated with the displacement of
+                the atoms during the minimization process.
+            max_disp (float): Maximum allowed atomic displacement in each
+                iteration.
+            spring_const (float): A virtual spring constant used in the NEB-like
+                        relaxation process that yields so-called IDPP path.
+            species (list of string): If provided, only those given species are
+                allowed to move. The atomic positions of other species are
+                obtained via regular linear interpolation approach.
+
+        Returns:
+            [Structure] Complete IDPP path (including end-point structures)
+        """
+
+        coords = self.init_coords.copy()
+        old_funcs = np.zeros((self.nimages,), dtype=np.float64)
+        idpp_structures = [self.structures[0]]
+
+        if species is None:
+            indices = list(range(len(self.structures[0])))
+        else:
+            species = [get_el_sp(sp) for sp in species]
+            indices = [
+                i for i, site in enumerate(self.structures[0]) if site.specie in species
+            ]
+
+            if len(indices) == 0:
+                raise ValueError("The given species are not in the system!")
+
+        # Iterative minimization
+        for n in range(maxiter):
+            # Get the sets of objective functions, true and total force
+            # matrices.
+            funcs, true_forces = self._get_funcs_and_forces(coords)
+            tot_forces = self._get_total_forces(
+                coords, true_forces, spring_const=spring_const
+            )
+
+            # Each atom is allowed to move up to max_disp
+            disp_mat = step_size * tot_forces[:, indices, :]
+            disp_mat = np.where(
+                np.abs(disp_mat) > max_disp, np.sign(disp_mat) * max_disp, disp_mat
+            )
+            coords[1 : (self.nimages + 1), indices] += disp_mat
+
+            max_force = np.abs(tot_forces[:, indices, :]).max()
+            tot_res = np.sum(np.abs(old_funcs - funcs))
+
+            if tot_res < tol and max_force < gtol:
+                break
+
+            old_funcs = funcs
+
+        else:
+            warnings.warn(
+                "Maximum iteration number is reached without convergence!", UserWarning
+            )
+
+        for ni in range(self.nimages):
+            # generate the improved image structure
+            new_sites = []
+
+            for site, cart_coords in zip(self.structures[ni + 1], coords[ni + 1]):
+                new_site = PeriodicSite(
+                    site.species,
+                    coords=cart_coords,
+                    lattice=site.lattice,
+                    coords_are_cartesian=True,
+                    properties=site.properties,
+                )
+                new_sites.append(new_site)
+
+            idpp_structures.append(Structure.from_sites(new_sites))
+
+        # Also include end-point structure.
+        idpp_structures.append(self.structures[-1])
+
+        return idpp_structures
+
+    @classmethod
+    def from_endpoints(cls, endpoints, nimages=5, sort_tol=1.0):
+        """
+        A class method that starts with end-point structures instead. The
+        initial guess for the IDPP algo is then constructed using linear
+        interpolation.
+
+        Args:
+            endpoints (list of Structure objects): The two end-point structures.
+            nimages (int): Number of images between the two end-points.
+            sort_tol (float): Distance tolerance (in Angstrom) used to match the
+                atomic indices between start and end structures. Need
+                to increase the value in some cases.
+        """
+        try:
+            images = endpoints[0].interpolate(
+                endpoints[1],
+                nimages=nimages + 1,
+                interpolate_lattices=True,
+                autosort_tol=sort_tol,
+            )
+        except Exception as e:
+            if "Unable to reliably match structures " in str(e):
+                warnings.warn(
+                    "Auto sorting is turned off because it is unable"
+                    " to match the end-point structures!",
+                    UserWarning,
+                )
+                images = endpoints[0].interpolate(
+                    endpoints[1], nimages=nimages + 1, autosort_tol=0
+                )
+            else:
+                raise e
+
+        return IDPPSolver(images)
+
+    def _get_funcs_and_forces(self, x):
+        """
+        Calculate the set of objective functions as well as their gradients,
+        i.e. "effective true forces"
+        """
+        funcs = []
+        funcs_prime = []
+        trans = self.translations
+        natoms = trans.shape[1]
+        weights = self.weights
+        target_dists = self.target_dists
+
+        for ni in range(len(x) - 2):
+            vec = [x[ni + 1, i] - x[ni + 1] - trans[ni, i] for i in range(natoms)]
+
+            trial_dist = np.linalg.norm(vec, axis=2)
+            aux = (
+                (trial_dist - target_dists[ni])
+                * weights[ni]
+                / (trial_dist + np.eye(natoms, dtype=np.float64))
+            )
+
+            # Objective function
+            func = np.sum((trial_dist - target_dists[ni]) ** 2 * weights[ni])
+
+            # "True force" derived from the objective function.
+            grad = np.sum(aux[:, :, None] * vec, axis=1)
+
+            funcs.append(func)
+            funcs_prime.append(grad)
+
+        return 0.5 * np.array(funcs), -2 * np.array(funcs_prime)
+
+    @staticmethod
+    def get_unit_vector(vec):
+        return vec / np.sqrt(np.sum(vec**2))
+
+    def _get_total_forces(self, x, true_forces, spring_const):
+        """
+        Calculate the total force on each image structure, which is equal to
+        the spring force along the tangent + true force perpendicular to the
+        tangent. Note that the spring force is the modified version in the
+        literature (e.g. Henkelman et al., J. Chem. Phys. 113, 9901 (2000)).
+        """
+
+        total_forces = []
+        natoms = np.shape(true_forces)[1]
+
+        for ni in range(1, len(x) - 1):
+            vec1 = (x[ni + 1] - x[ni]).flatten()
+            vec2 = (x[ni] - x[ni - 1]).flatten()
+
+            # Local tangent
+            tangent = self.get_unit_vector(vec1) + self.get_unit_vector(vec2)
+            tangent = self.get_unit_vector(tangent)
+
+            # Spring force
+            spring_force = (
+                spring_const * (np.linalg.norm(vec1) - np.linalg.norm(vec2)) * tangent
+            )
+
+            # Total force
+            flat_ft = true_forces[ni - 1].copy().flatten()
+            total_force = true_forces[ni - 1] + (
+                spring_force - np.dot(flat_ft, tangent) * tangent
+            ).reshape(natoms, 3)
+            total_forces.append(total_force)
+
+        return np.array(total_forces)
```

## dspawpy/io/read.py

```diff
@@ -1,1339 +1,1513 @@
-"""
-Functions to read properties from structure or output files
-"""
-
-import json
-import os
-import re
-
-import h5py
-import numpy as np
-from pymatgen.core.lattice import Lattice
-from pymatgen.core.structure import Structure
-from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
-from pymatgen.electronic_structure.core import Orbital, Spin
-from pymatgen.electronic_structure.dos import CompleteDos, Dos
-from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine
-from pymatgen.phonon.dos import PhononDos
-
-
-def get_band_data(
-    band_dir: str,
-    syst_dir: str = None,
-    efermi: float = None,
-    zero_to_efermi: bool = False,
-) -> BandStructureSymmLine:
-    """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
-
-    Parameters
-    ----------
-    band_dir : str
-        能带文件路径，band.h5 / band.json
-    syst_dir : str
-        system.json 路径，仅为辅助处理 Wannier 数据而准备
-    efermi : float, optional
-        费米能级，如果h5文件中的费米能级不正确，可以通过此参数指定费米能级
-    zero_to_efermi : bool, optional
-        是否将费米能级移动到0
-
-    Returns
-    -------
-    BandStructureSymmLine
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import get_band_data
-    >>> band = get_band_data(band_dir='/data/home/hzw1002/dspawpy_repo/test/2.3/band.h5')
-
-    如果希望通过指定wannier.json来处理瓦尼尔能带，需要额外指定syst_dir参数
-
-    >>> band = get_band_data(band_dir='/data/home/hzw1002/dspawpy_repo/test/2.30/wannier.json', syst_dir='/data/home/hzw1002/dspawpy_repo/test/2.30/system.json')
-    """
-    if efermi is not None and zero_to_efermi:
-        raise ValueError(
-            "efermi and zero_to_efermi should not be set at the same time!"
-        )
-    if band_dir.endswith(".h5"):
-        band = load_h5(band_dir)
-        raw = h5py.File(band_dir, "r").keys()
-        if "/WannBandInfo/NumberOfBand" in raw:
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = _get_band_data_h5(band, iwan=True, zero_to_efermi=zero_to_efermi)
-        elif "/BandInfo/NumberOfBand" in raw:
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = _get_band_data_h5(band, iwan=False, zero_to_efermi=zero_to_efermi)
-        else:
-            print("BandInfo or WannBandInfo key not found in h5file!")
-            return
-    elif band_dir.endswith(".json"):
-        with open(band_dir, "r") as fin:
-            band = json.load(fin)
-        if "WannBandInfo" in band.keys():
-            assert (
-                syst_dir is not None
-            ), "system.json is required for processing wannier band info!"
-            with open(syst_dir) as system_json:
-                syst = json.load(system_json)
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = _get_band_data_json(
-                band, syst, iwan=True, zero_to_efermi=zero_to_efermi
-            )
-        elif "BandInfo" in band.keys():
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = _get_band_data_json(band, iwan=False, zero_to_efermi=zero_to_efermi)
-        else:
-            print("BandInfo or WannBandInfo key not found in json file!")
-            return
-    else:
-        raise TypeError(f"{os.path.abspath(band_dir)} must be h5 or json file!")
-
-    if efermi:  # 从h5直接读取的费米能级可能是错的，此时需要用户自行指定
-        rEf = efermi  # 这只是个临时解决方案
-
-    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
-    return BandStructureSymmLine(
-        kpoints=kpoints,
-        eigenvals=eigenvals,
-        lattice=lattice_new,
-        efermi=rEf,
-        labels_dict=labels_dict,
-        structure=structure,
-        projections=projections,
-    )
-
-
-def get_dos_data(dos_dir: str) -> CompleteDos or Dos:
-    """读取h5或json文件中的态密度数据，构建CompleteDos或DOS对象
-
-    Parameters
-    ----------
-    dos_dir : str
-        态密度文件路径，dos.h5 / dos.json
-
-    Returns
-    -------
-    CompleteDos or Dos
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import get_dos_data
-    >>> dos = get_dos_data(dos_dir='/data/home/hzw1002/dspawpy_repo/test/2.5/dos.h5')
-    """
-    if dos_dir.endswith(".h5"):
-        dos = load_h5(dos_dir)
-        if dos["/DosInfo/Project"][0]:
-            return _get_complete_dos(dos)
-        else:
-            return _get_total_dos(dos)
-
-    elif dos_dir.endswith(".json"):
-        with open(dos_dir, "r") as fin:
-            dos = json.load(fin)
-
-        if dos["DosInfo"]["Project"]:
-            return _get_complete_dos_json(dos)
-        else:
-            return _get_total_dos_json(dos)
-
-    else:
-        raise TypeError(f"{os.path.abspath(dos_dir)} must be h5 or json file!")
-
-
-def get_ele_from_h5(hpath: str = "aimd.h5"):
-    """从h5文件中读取元素列表；
-    多离子步并不会在每个离子步的Structure中保存元素信息，只能读取初始结构的元素信息
-
-    Parameters
-    ----------
-    hpath : str
-        h5文件路径
-
-    Returns
-    -------
-    ele : list
-        元素列表, Natom x 1
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import get_ele_from_h5
-    >>> ele = get_ele_from_h5(hpath='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5')
-    >>> ele
-    ['H', 'H_1', 'O']
-    """
-    data = h5py.File(hpath)
-    Elements_bytes = np.array(data.get("/AtomInfo/Elements"))
-    tempdata = np.array([i.decode() for i in Elements_bytes])
-    ele = "".join(tempdata).split(";")
-
-    return ele
-
-
-def get_lines_without_comment(filename: str, comment: str = "#"):
-    """读取as文件内容，移除批注后返回行列表
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import get_lines_without_comment
-    >>> lines = get_lines_without_comment(filename='/data/home/hzw1002/dspawpy_repo/test/2.15/01/structure01.as', comment='#')
-    >>> lines
-    ['Total number of atoms', '13', 'Lattice', '5.60580000 0.00000000 0.00000000', '0.00000000 5.60580000 0.00000000', '0.00000000 0.00000000 16.81740000', 'Cartesian', 'H 2.48700709 3.85367720 6.93461994', 'Pt 1.40145000 1.40145000 1.98192999', 'Pt 4.20434996 1.40145000 1.98192999', 'Pt 1.40145000 4.20434996 1.98192999', 'Pt 4.20434996 4.20434996 1.98192999', 'Pt 0.00843706 0.00042409 3.91500875', 'Pt 0.00881029 2.80247953 3.91551673', 'Pt 2.81216310 -0.00105882 3.91807627', 'Pt 2.81156629 2.80392163 3.91572506', 'Pt 1.41398585 1.39603492 5.85554462', 'Pt 4.22886663 1.39820574 5.84677553', 'Pt 1.40485707 4.20963461 5.89521929', 'Pt 4.23788559 4.20753128 5.88625580']
-    """
-    lines = []
-    """Filter out comment lines"""
-    with open(filename) as file:
-        while True:
-            line = file.readline()
-            if line:
-                line = re.sub(comment + r".*$", "", line)  # remove comment
-                line = line.strip()
-                if line:
-                    lines.append(line)
-            else:
-                break
-
-    return lines
-
-
-def get_phonon_band_data(phonon_band_dir: str) -> PhononBandStructureSymmLine:
-    """读取h5或json文件中的声子能带数据，构建PhononBandStructureSymmLine对象
-
-    Parameters
-    ----------
-    phonon_band_dir : str
-        能带文件路径，phonon.h5 / phonon.json
-
-    Returns
-    -------
-    PhononBandStructureSymmLine
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import get_phonon_band_data
-    >>> band_data = get_phonon_band_data("/data/home/hzw1002/dspawpy_repo/test//2.16/phonon.h5") # 读取声子能带
-    """
-    if phonon_band_dir.endswith(".h5"):
-        band = load_h5(phonon_band_dir)
-        (
-            symmmetry_kpoints,
-            symmetry_kPoints_index,
-            kpoints,
-            structure,
-            frequencies,
-        ) = _get_phonon_band_data_h5(band)
-    elif phonon_band_dir.endswith(".json"):
-        with open(phonon_band_dir, "r") as fin:
-            band = json.load(fin)
-        (
-            symmmetry_kpoints,
-            symmetry_kPoints_index,
-            kpoints,
-            structure,
-            frequencies,
-        ) = _get_phonon_band_data_json(band)
-    else:
-        raise TypeError(f"{os.path.abspath(phonon_band_dir)} must be h5 or json file")
-
-    labels_dict = {}
-    for i, s in enumerate(symmmetry_kpoints):
-        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
-    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
-
-    return PhononBandStructureSymmLine(
-        qpoints=kpoints,
-        frequencies=frequencies,
-        lattice=lattice_new,
-        has_nac=False,
-        labels_dict=labels_dict,
-        structure=structure,
-    )
-
-
-def get_phonon_dos_data(phonon_dos_dir: str) -> PhononDos:
-    """读取h5或json文件中的声子态密度数据，构建PhononDos对象
-
-    Parameters
-    ----------
-    phonon_dos_dir : str
-        声子态密度文件路径，phonon_dos.h5 / phonon_dos.json
-
-    Returns
-    -------
-    PhononDos
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import get_phonon_dos_data
-    >>> phdos = get_phonon_dos_data(phonon_dos_dir='/data/home/hzw1002/dspawpy_repo/test/2.16.1/phonon.h5')
-    >>> phdos.frequencies
-    array([ 0. ,  0.1,  0.2,  0.3,  0.4,  0.5,  0.6,  0.7,  0.8,  0.9,  1. ,
-            1.1,  1.2,  1.3,  1.4,  1.5,  1.6,  1.7,  1.8,  1.9,  2. ,  2.1,
-            2.2,  2.3,  2.4,  2.5,  2.6,  2.7,  2.8,  2.9,  3. ,  3.1,  3.2,
-            3.3,  3.4,  3.5,  3.6,  3.7,  3.8,  3.9,  4. ,  4.1,  4.2,  4.3,
-            4.4,  4.5,  4.6,  4.7,  4.8,  4.9,  5. ,  5.1,  5.2,  5.3,  5.4,
-            5.5,  5.6,  5.7,  5.8,  5.9,  6. ,  6.1,  6.2,  6.3,  6.4,  6.5,
-            6.6,  6.7,  6.8,  6.9,  7. ,  7.1,  7.2,  7.3,  7.4,  7.5,  7.6,
-            7.7,  7.8,  7.9,  8. ,  8.1,  8.2,  8.3,  8.4,  8.5,  8.6,  8.7,
-            8.8,  8.9,  9. ,  9.1,  9.2,  9.3,  9.4,  9.5,  9.6,  9.7,  9.8,
-            9.9, 10. , 10.1, 10.2, 10.3, 10.4, 10.5, 10.6, 10.7, 10.8, 10.9,
-           11. , 11.1, 11.2, 11.3, 11.4, 11.5, 11.6, 11.7, 11.8, 11.9, 12. ,
-           12.1, 12.2, 12.3, 12.4, 12.5, 12.6, 12.7, 12.8, 12.9, 13. , 13.1,
-           13.2, 13.3, 13.4, 13.5, 13.6, 13.7, 13.8, 13.9, 14. , 14.1, 14.2,
-           14.3, 14.4, 14.5, 14.6, 14.7, 14.8, 14.9, 15. , 15.1, 15.2, 15.3,
-           15.4, 15.5, 15.6, 15.7, 15.8, 15.9, 16. , 16.1, 16.2, 16.3, 16.4,
-           16.5, 16.6, 16.7, 16.8, 16.9, 17. , 17.1, 17.2, 17.3, 17.4, 17.5,
-           17.6, 17.7, 17.8, 17.9, 18. , 18.1, 18.2, 18.3, 18.4, 18.5, 18.6,
-           18.7, 18.8, 18.9, 19. , 19.1, 19.2, 19.3, 19.4, 19.5, 19.6, 19.7,
-           19.8, 19.9, 20. ])
-    """
-    if phonon_dos_dir.endswith(".h5"):
-        dos = load_h5(phonon_dos_dir)
-        frequencies = np.asarray(dos["/DosInfo/DosEnergy"])
-        densities = dos["/DosInfo/Spin1/Dos"]
-    elif phonon_dos_dir.endswith(".json"):
-        with open(phonon_dos_dir, "r") as fin:
-            dos = json.load(fin)
-        frequencies = np.asarray(dos["DosInfo"]["DosEnergy"])
-        densities = dos["DosInfo"]["Spin1"]["Dos"]
-    else:
-        raise TypeError(f"{os.path.abspath(phonon_dos_dir)} must be h5 or json file")
-
-    return PhononDos(frequencies, densities)
-
-
-def get_sinfo(datafile: str, scaled=False, si=None, ele=None, ai=None):
-    r"""Wrapper to get structure information from h5/json/as file.
-
-    从datafile中读取结构信息
-
-    Parameters
-    ----------
-    datafile : str
-        h5 / json 文件路径
-    scaled : bool, optional
-        是否返回分数坐标，默认False
-    si : int or list or str, optional
-        运动轨迹中的第几步，从1开始计数！
-        如果要切片，用字符串写法： '1, 10'
-        默认为None，返回所有步
-    ele : list, optional
-        元素列表, Natom x 1
-        默认为None，从h5文件中读取
-    ai : int or list or str, optional
-        多离子步中的第几个离子步，从1开始计数
-        如果要切片，用字符串写法： '1, 10'
-        默认为None，返回所有离子步
-
-    Returns
-    -------
-    Nstep : int
-        总离子步数（几个构型）
-    ele : list
-        元素列表, Natom x 1
-    pos : np.ndarray
-        坐标分量数组，Nstep x Natom x 3
-    latv : np.ndarray
-        晶胞矢量数组，Nstep x 3 x 3
-    D_mag_fix : dict
-        磁矩、自由度相关信息
-
-    Examples
-    --------
-
-    >>> from dspawpy.io.read import get_sinfo
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', scaled=False, si=None, ele=None, ai=None)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='/data/home/hzw1002/dspawpy_repo/test/2.1/relax.json', scaled=False, si=None, ele=None, ai=None)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.1/relax.json...
-     json所含数据仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！
-    Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info...
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='/data/home/hzw1002/dspawpy_repo/test/2.2/rho.json', scaled=False)
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.2/rho.json...
-     json所含数据仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！
-
-    这些信息可以用于进一步构建Structure对象，
-    具体参考 dspawpy.io.structure.build_Structures_from_datafile 函数
-    """
-    if datafile.endswith(".h5"):
-        assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
-        hpath = datafile
-        print(f"Reading {os.path.abspath(hpath)}...")
-        hf = h5py.File(hpath)  # 加载h5文件
-
-        # decide task type by check the internal key
-        if "/Structures" in hf.keys():  # multi-steps
-            Total_step = np.array(hf.get("/Structures/FinalStep"))[0]  # 总步数
-
-            if ele is not None and ai is not None:
-                raise ValueError("暂不支持同时指定元素和原子序号")
-            # 步数
-            if si is not None:
-                if isinstance(si, int):  # 1
-                    indices = [si]
-
-                elif isinstance(si, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                    indices = si
-
-                elif isinstance(si, str):  # ':', '-3:'
-                    indices = __parse_indices(si, Total_step)
-
-                else:
-                    raise ValueError("请输入正确格式的index")
-
-                Nstep = len(indices)
-            else:
-                Nstep = Total_step
-                indices = list(range(1, Nstep + 1))
-
-            # 读取元素列表，这个列表不会随步数改变，也不会“合并同类项”
-            Elements = np.array(get_ele_from_h5(hpath), dtype=object)
-
-            # 开始读取晶胞和原子位置
-            lattices = np.empty((Nstep, 3, 3))  # Nstep x 3 x 3
-            location = []
-            if ele is not None:  # 如果用户指定元素
-                if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
-                    ele_list = np.array(ele, dtype=object)
-                    location = np.where(Elements == ele_list)[0]
-                # 多个元素符号组成的列表，例如 ['Fe', 'O']
-                elif isinstance(ele, list) or isinstance(ele, np.ndarray):
-                    for e in ele:
-                        loc = np.where(Elements == e)[0]
-                        location.append(loc)
-                    location = np.concatenate(location)
-                else:
-                    raise TypeError("请输入正确的元素或元素列表")
-                elements = Elements[location]
-
-            elif ai is not None:  # 如果用户指定原子序号
-                if isinstance(ai, int):  # 1
-                    ais = [ai]
-                elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                    ais = ai
-                elif isinstance(ai, str):  # ':', '-3:'
-                    ais = __parse_indices(ai, Total_step)
-                else:
-                    raise ValueError("请输入正确格式的ai")
-                ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
-                elements = Elements[ais]
-                location = ais
-
-            else:  # 如果都没指定
-                elements = Elements
-                location = list(range(len(Elements)))
-
-            elements = elements.tolist()  # for pretty output
-            Natom = len(elements)
-            mags = []  # must be Nstep x Natom x ?
-
-            poses = np.empty(shape=(len(indices), Natom, 3))
-            wrapped_poses = np.empty(shape=(len(indices), 3, Natom))
-            for i, ind in enumerate(indices):  # 步数
-                # print(f'{ind=}')
-                lats = np.array(hf.get("/Structures/Step-" + str(ind) + "/Lattice"))
-                lattices[i] = lats
-                # [x1,y1,z1,x2,y2,z2,x3,y3,z3], ...
-                # 结构优化时输出的都是分数坐标，不管CoordinateType写的是啥！
-                pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
-                wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
-                wrapped_pos = (
-                    wrapped_pos.flatten().reshape(-1, 3).T
-                )  # reshape to 3 x Natom
-                wrapped_poses[i] = wrapped_pos
-
-                iNoncollinear = False
-                try:  # 自旋计算
-                    if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
-                        mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
-                    elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
-                        magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
-                        magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
-                        magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
-                        iNoncollinear = True
-                    else:
-                        mag = np.zeros(shape=(Natom, 1))
-
-                except Exception as e:
-                    if str(e):  # ignore empty AssertionError()
-                        print(e)
-                    mag = np.zeros(shape=(Natom, 1))
-
-                mags.append(mag)
-
-            if "/AtomInfo/Fix" in hf.keys():  # fix atom
-                atomFixs_raw = np.array(hf.get("/AtomInfo/Fix"))
-                atomFixs = np.array(
-                    ["True" if _v else "False" for _v in atomFixs_raw]
-                ).reshape(-1, 3)
-            else:
-                atomFixs = np.full(shape=(Natom, 3), fill_value="False")
-
-            try:  # fix lattice
-                latticeFixs = (
-                    np.array(hf.get("/AtomInfo/FixLattice")).astype(bool).flatten()
-                )
-                assert latticeFixs.shape == (9,)
-                latticeFixs = latticeFixs.reshape(
-                    9,
-                )  # (9,)
-            except Exception as e:
-                if str(e):  # ignore empty AssertionError()
-                    print(e)
-                latticeFixs = np.full(shape=(9,), fill_value="False")
-
-            # repeat atomFixs of shape Natom x 3 to Nstep x Natom x 3
-            atomFixs = np.repeat(atomFixs[np.newaxis, :], Nstep, axis=0).reshape(
-                Nstep, Natom, 3
-            )
-
-            # repeat latticeFixs of shape 9 x 1 to Nstep x Natom x 9
-            latticeFixs = (
-                np.repeat(latticeFixs[np.newaxis, :], Nstep * Natom, axis=0)
-                .reshape(Nstep, Natom, 9)
-                .tolist()
-            )
-
-            if iNoncollinear == False:
-                mags = np.array(mags).reshape(Nstep, Natom, -1).tolist()
-                D_mag_fix = {
-                    "Mag": mags,
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-            else:
-                D_mag_fix = {
-                    "Mag_x": magx,
-                    "Mag_y": magy,
-                    "Mag_z": magz,
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-
-            if scaled:  # Fractional coordinates
-                for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):  # atom si
-                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
-            else:  # Cartesian coordinates
-                for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):
-                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
-
-        elif "/UnrelaxStructure" in hf.keys():  # single-step
-            raise NotImplementedError(
-                "Read from neb.h5 is not implemented yet!\n you may try neb01.h5.."
-            )
-        elif "/UnitAtomInfo" in hf.keys():  # phonon
-            raise NotImplementedError(
-                "Read from phonon.h5 is not implemented yet!\n you may try phonon001.h5.."
-            )
-        else:  # rho, potential, elf, pcharge
-            hfDict = load_h5(hpath)
-            s = _get_structure(hfDict, "/AtomInfo")
-            elements = s.species
-            poses = [s.cart_coords]
-            lattices = [s.lattice.matrix]
-            Nstep = 1
-            D_mag_fix = None
-            print("--> rho/potential/elf/pcharge.h5 has no mag or fix info,")
-            print("  you should manually set it before starting new calculations..")
-
-    elif datafile.endswith(".json"):
-        assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
-        jpath = datafile
-        print(f"Reading {os.path.abspath(jpath)}...")
-        print(f" json所含数据仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！")
-        with open(jpath, "r") as f:
-            data = json.load(f)  # 加载json文件
-
-        # decide the task type by checking the internal keys
-        if "AtomInfo" in data:  # single-step task
-            s = _get_structure_json(data["AtomInfo"])
-            elements = s.species
-            poses = [s.cart_coords]
-            lattices = [s.lattice.matrix]
-            Nstep = 1
-            D_mag_fix = None
-
-        elif "UnitAtomInfo" in data:  # phonon task
-            raise NotImplementedError("Read from phonon.json is not supported yet.")
-        elif "IniFin" in data:  # neb.json
-            raise NotImplementedError("Read from neb.json is not supported yet.")
-        elif "WannierInfo" in data:
-            raise NotImplementedError("wannier.json has no stucture info!")
-
-        else:  # multi-steps task
-            if "Structures" in data:
-                Total_step = len(data["Structures"])  # aimd.json
-            else:
-                Total_step = len(data)  # relax.json, neb01.json
-
-            if ele is not None and ai is not None:
-                raise ValueError("暂不支持同时指定元素和原子序号")
-            # 步数
-            if si is not None:
-                if isinstance(si, int):  # 1
-                    indices = [si]
-
-                elif isinstance(si, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                    indices = si
-
-                elif isinstance(si, str):  # ':', '-3:'
-                    indices = __parse_indices(si, Total_step)
-
-                else:
-                    raise ValueError("请输入正确格式的index")
-
-                Nstep = len(indices)
-            else:
-                Nstep = Total_step
-                indices = list(range(1, Nstep + 1))  # [1,Nstep+1)
-
-            # 预先读取全部元素的总列表，这个列表不会随步数改变，也不会“合并同类项”
-            # 这样可以避免在循环内部频繁判断元素是否符合用户需要
-
-            if "Structures" in data:
-                Nele = len(data["Structures"][0]["Atoms"])  # relax.json
-                total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
-                for i in range(Nele):
-                    element = data["Structures"][0]["Atoms"][i]["Element"]
-                    total_elements[i] = element
-            else:
-                if "Atoms" not in data[0]:
-                    raise NotImplementedError("nebXX.json has no structure info!")
-                Nele = len(data[0]["Atoms"])
-                total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
-                for i in range(Nele):
-                    element = data[0]["Atoms"][i]["Element"]
-                    total_elements[i] = element
-
-            Natom = len(total_elements)
-
-            # 开始读取晶胞和原子位置
-            # 在data['Structures']['%d' % index]['Atoms']中根据元素所在序号选择结构
-            if ele is not None:  # 用户指定要某些元素
-                location = []
-                if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
-                    ele_list = list(ele)
-                # 多个元素符号组成的列表，例如 ['Fe', 'O']
-                elif isinstance(ele, list) or isinstance(ele, np.ndarray):
-                    ele_list = ele
-                else:
-                    raise TypeError("请输入正确的元素或元素列表")
-                for e in ele_list:
-                    location.append(np.where(total_elements == e)[0])
-                location = np.concatenate(location)
-
-            elif ai is not None:  # 如果用户指定原子序号，也要据此筛选元素列表
-                if isinstance(ai, int):  # 1
-                    ais = [ai]
-                elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                    ais = ai
-                elif isinstance(ai, str):  # ':', '-3:'
-                    ais = __parse_indices(ai, Total_step)
-                else:
-                    raise ValueError("请输入正确格式的ai")
-                ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
-                location = ais
-                # read lattices and poses
-
-            else:  # 如果都没指定
-                location = list(range(Natom))
-
-            # 满足用户需要的elements列表
-            elements = np.empty(shape=(Natom,), dtype=object)
-            for i in range(len(location)):
-                elements[i] = total_elements[location[i]]
-
-            # Nstep x Natom x 3, positions are all fractional
-            poses = np.empty(shape=(len(indices), len(elements), 3))
-            lattices = np.empty(shape=(Nstep, 3, 3))  # Nstep x 3 x 3
-            mags = []  # Nstep x Natom x ?
-            Atomfixs = []  # Nstep x Natom x 1
-            LatFixs = []  # Nstep x Natom x 9
-
-            if "Structures" in data:  # aimd
-                for i, ind in enumerate(indices):  # for every ionic step
-                    lat = data["Structures"][ind - 1]["Lattice"]
-                    lattices[i] = np.array(lat).reshape(3, 3)
-                    mag_for_each_step = []
-                    fix_for_each_step = []
-                    if "FixLattice" in data["Structures"][ind - 1]:
-                        fixlat_raw = data["Structures"][ind - 1]["FixLattice"]
-                    else:
-                        fixlat_raw = []
-                    if fixlat_raw == []:
-                        fixlat_raw = np.full((9, 1), fill_value=False).tolist()
-                    fixlat_str = [
-                        "True" if _v == True else "False" for _v in fixlat_raw
-                    ]
-                    fixlat_arr = np.array(fixlat_str).reshape(9, 1)
-                    # repeat fixlat for each atom
-                    fixlat = np.repeat(fixlat_arr, Natom, axis=1).T.tolist()
-                    LatFixs.append(fixlat)
-                    for j, sli in enumerate(location):
-                        ati = data["Structures"][ind - 1]["Atoms"][sli]
-                        poses[i, j, :] = ati["Position"][:]
-
-                        mag_for_each_atom = ati["Mag"][:]
-                        if mag_for_each_atom == []:
-                            mag_for_each_atom = [0.0]
-                        mag_for_each_step.append(mag_for_each_atom)
-
-                        fix_for_each_atom = ati["Fix"][:]
-                        if fix_for_each_atom == []:
-                            fix_for_each_atom = ["False"]
-                        fix_for_each_step.append(fix_for_each_atom)
-
-                    mags.append(mag_for_each_step)
-                    Atomfixs.append(fix_for_each_step)
-                    if not scaled:
-                        poses[i] = np.dot(poses[i], lattices[i])
-
-            else:  # relax, neb01
-                print(
-                    "Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info..."
-                )
-
-                for i, ind in enumerate(indices):  # for every ionic step
-                    lat = data[ind - 1]["Lattice"]
-                    lattices[i] = np.array(lat).reshape(3, 3)
-                    mag_for_each_step = []
-                    fix_for_each_step = []
-                    if "FixLattice" in data[ind - 1]:
-                        fixlat_raw = data[ind - 1]["FixLattice"]
-                        if fixlat_raw == None:
-                            fixlat_raw = np.full((9, 1), fill_value=False).tolist()
-                        fixlat_str = [
-                            "True" if _v == True else "False" for _v in fixlat_raw
-                        ]
-                        fixlat_arr = np.array(fixlat_str).reshape(9, 1)
-                        # repeat fixlat for each atom
-                        fixlat = np.repeat(fixlat_arr, Natom, axis=1).T.tolist()
-                    else:
-                        fixlat = np.full((Natom, 9), fill_value=False).tolist()
-
-                    LatFixs.append(fixlat)
-                    for j, sli in enumerate(location):
-                        ati = data[ind - 1]["Atoms"][sli]
-                        poses[i, j, :] = ati["Position"][:]
-
-                        mag_for_each_atom = ati["Mag"][:]
-                        if mag_for_each_atom == []:
-                            mag_for_each_atom = [0.0]
-                        mag_for_each_step.append(mag_for_each_atom)
-
-                        fix_for_each_atom = ati["Fix"][:]
-                        if fix_for_each_atom == []:
-                            fix_for_each_atom = ["False"]
-                        fix_for_each_step.append(fix_for_each_atom)
-
-                    mags.append(mag_for_each_step)
-                    Atomfixs.append(fix_for_each_step)
-                    if not scaled:
-                        poses[i] = np.dot(poses[i], lattices[i])
-
-            elements = elements.tolist()
-            Mags = np.array(mags).tolist()  # (Nstep, Natom, ?) or (Nstep, 0,)
-
-            D_mag_fix = {"Mag": Mags, "Fix": Atomfixs, "LatticeFixs": LatFixs}
-
-    else:
-        raise ValueError(
-            "get_sinfo function only accept datafile of .h5 / .json format!"
-        )
-
-    return Nstep, elements, poses, lattices, D_mag_fix
-
-
-def load_h5(dir_h5: str) -> dict:
-    """遍历读取h5文件中的数据，保存为字典格式
-
-    慎用此函数，因为会读取很多不需要的数据，耗时很长。
-
-    Parameters
-    ----------
-    dir_h5 : str
-        h5文件路径
-
-    Returns
-    -------
-    datas: dict
-        数据字典
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import load_h5
-    >>> datas = load_h5(dir_h5='/data/home/hzw1002/dspawpy_repo/test/2.2/scf.h5')
-    >>> datas.keys()
-    dict_keys(['/AtomInfo/CoordinateType', '/AtomInfo/Elements', '/AtomInfo/Grid', '/AtomInfo/Lattice', '/AtomInfo/Position', '/Eigenvalue/CBM/BandIndex', '/Eigenvalue/CBM/Energy', '/Eigenvalue/CBM/Kpoint', '/Eigenvalue/NumberOfBand', '/Eigenvalue/Spin1/BandEnergies', '/Eigenvalue/Spin1/Kpoints/Coordinates', '/Eigenvalue/Spin1/Kpoints/Grid', '/Eigenvalue/Spin1/Kpoints/NumberOfKpoints', '/Eigenvalue/Spin1/Occupation', '/Eigenvalue/VBM/BandIndex', '/Eigenvalue/VBM/Energy', '/Eigenvalue/VBM/Kpoint', '/Electron', '/Energy/EFermi', '/Energy/TotalEnergy', '/Energy/TotalEnergy0', '/Force/ForceOnAtoms', '/Stress/Direction', '/Stress/Pressure', '/Stress/Stress', '/Stress/Total', '/Structures/FinalStep', '/Structures/Step-1/Lattice', '/Structures/Step-1/Position'])
-    """
-
-    def get_names(key, h5_object):
-        names.append(h5_object.name)
-
-    def is_dataset(name):
-        for name_inTheList in names:
-            if name_inTheList.find(name + "/") != -1:
-                return False
-        return True
-
-    def get_datas(key, h5_object):
-        if is_dataset(h5_object.name):
-            data = np.asarray(h5_object)
-            if data.dtype == "|S1":  # 转成字符串 并根据";"分割
-                byte2str = [str(bi, "utf-8") for bi in data]
-                string = ""
-                for char in byte2str:
-                    string += char
-                data = np.array([elem for elem in string.strip().split(";")])
-            # "/group1/group2/.../groupN/dataset" : value
-            datas[h5_object.name] = data.tolist()
-
-    with h5py.File(dir_h5, "r") as fin:
-        names = []
-        datas = {}
-        fin.visititems(get_names)
-        fin.visititems(get_datas)
-
-        return datas
-
-
-def load_h5_todict(dir_h5: str) -> dict:
-    """与上一个函数区别在于合并了部分同类数据，例如
-
-    /Structures/Step-1/* 和 /Structures/Step-2/* 并入 /Structures/ 组内
-    """
-
-    def create_dict(L: list, D: dict):
-        if len(L) == 2:
-            D[L[0]] = L[1]
-            return
-        else:
-            if not (L[0] in D.keys()):
-                D[L[0]] = {}
-            create_dict(L[1:], D[L[0]])
-
-    datas = load_h5(dir_h5)
-
-    groups_value_list = []
-    for key in datas.keys():
-        tmp_list = key[1:].strip().split("/")  # [1:] 截去root
-        tmp_list.append(datas[key])
-        # groups_value_list[i]结构: [group1, group2, ..., groupN, dataset, value]
-        groups_value_list.append(tmp_list)
-
-    groups_value_dict = {}
-    for data in groups_value_list:
-        create_dict(data, groups_value_dict)
-
-    return groups_value_dict
-
-
-def __parse_indices(index: str, total_step) -> list:
-    """解析用户输入的原子序号字符串
-
-    输入：
-        - index: 用户输入的原子序号/元素字符串，例如 '1:3,5,7:10'
-    输出：
-        - indices: 解析后的原子序号列表，例如 [1,2,3,4,5,6,7,8,9,10]
-    """
-    assert ":" in index, "如果不想切片索引，请输入整数或者列表"
-    blcs = index.split(",")
-    indices = []
-    for blc in blcs:
-        if ":" in blc:  # 切片
-            low = blc.split(":")[0]
-            if not low:
-                low = 1  # 从1开始
-            else:
-                low = int(low)
-                assert low > 0, "索引从1开始！"
-            high = blc.split(":")[1]
-            if not high:
-                high = total_step
-            else:
-                high = int(high)
-                assert high <= total_step, "索引超出范围！"
-
-            for i in range(low, high + 1):
-                indices.append(i)
-        else:  # 单个数字
-            indices.append(int(blc))
-    return indices
-
-
-def _get_lammps_non_orthogonal_box(lat: np.ndarray):
-    """计算用于输入lammps的盒子边界参数，用于生成dump结构文件
-
-    Parameters
-    ----------
-    lat : np.ndarray
-        常见的非三角3x3矩阵
-
-    Returns
-    -------
-    box_bounds:
-        用于输入lammps的盒子边界
-    """
-    # https://docs.lammps.org/Howto_triclinic.html
-    A = lat[0]
-    B = lat[1]
-    C = lat[2]
-    assert np.cross(A, B).dot(C) > 0, "Lat is not right handed"
-
-    # 将常规3x3矩阵转成标准的上三角矩阵
-    alpha = np.arccos(np.dot(B, C) / (np.linalg.norm(B) * np.linalg.norm(C)))
-    beta = np.arccos(np.dot(A, C) / (np.linalg.norm(A) * np.linalg.norm(C)))
-    gamma = np.arccos(np.dot(A, B) / (np.linalg.norm(A) * np.linalg.norm(B)))
-
-    ax = np.linalg.norm(A)
-    a = np.array([ax, 0, 0])
-
-    bx = np.linalg.norm(B) * np.cos(gamma)
-    by = np.linalg.norm(B) * np.sin(gamma)
-    b = np.array([bx, by, 0])
-
-    cx = np.linalg.norm(C) * np.cos(beta)
-    cy = (np.linalg.norm(B) * np.linalg.norm(C) - bx * cx) / by
-    cz = np.sqrt(abs(np.linalg.norm(C) ** 2 - cx**2 - cy**2))
-    c = np.array([cx, cy, cz])
-
-    # triangluar matrix in lammmps cell format
-    # note that in OVITO, it will be down-triangular one
-    # lammps_lattice = np.array([a,b,c]).T
-
-    # write lammps box parameters
-    # https://docs.lammps.org/Howto_triclinic.html#:~:text=The%20inverse%20relationship%20can%20be%20written%20as%20follows
-    lx = np.linalg.norm(a)
-    xy = np.linalg.norm(b) * np.cos(gamma)
-    xz = np.linalg.norm(c) * np.cos(beta)
-    ly = np.sqrt(np.linalg.norm(b) ** 2 - xy**2)
-    yz = (np.linalg.norm(b) * np.linalg.norm(c) * np.cos(alpha) - xy * xz) / ly
-    lz = np.sqrt(np.linalg.norm(c) ** 2 - xz**2 - yz**2)
-
-    # "The parallelepiped has its “origin” at (xlo,ylo,zlo) and is defined by 3 edge vectors starting from the origin given by a = (xhi-xlo,0,0); b = (xy,yhi-ylo,0); c = (xz,yz,zhi-zlo)."
-    # 令原点在(0,0,0)，则 xlo = ylo = zlo = 0
-    xlo = ylo = zlo = 0
-    # https://docs.lammps.org/Howto_triclinic.html#:~:text=the%20LAMMPS%20box%20sizes%20(lx%2Cly%2Clz)%20%3D%20(xhi%2Dxlo%2Cyhi%2Dylo%2Czhi%2Dzlo)
-    xhi = lx + xlo
-    yhi = ly + ylo
-    zhi = lz + zlo
-    # https://docs.lammps.org/Howto_triclinic.html#:~:text=This%20bounding%20box%20is%20convenient%20for%20many%20visualization%20programs%20and%20is%20calculated%20from%20the%209%20triclinic%20box%20parameters%20(xlo%2Cxhi%2Cylo%2Cyhi%2Czlo%2Czhi%2Cxy%2Cxz%2Cyz)%20as%20follows%3A
-    xlo_bound = xlo + np.min([0, xy, xz, xy + xz])
-    xhi_bound = xhi + np.max([0, xy, xz, xy + xz])
-    ylo_bound = ylo + np.min([0, yz])
-    yhi_bound = yhi + np.max([0, yz])
-    zlo_bound = zlo
-    zhi_bound = zhi
-    box_bounds = np.array(
-        [
-            [xlo_bound, xhi_bound, xy],
-            [ylo_bound, yhi_bound, xz],
-            [zlo_bound, zhi_bound, yz],
-        ]
-    )
-
-    return box_bounds
-
-
-def _get_total_dos(dos: dict) -> Dos:
-    # h5 -> Dos Obj
-    energies = np.asarray(dos["/DosInfo/DosEnergy"])
-    if dos["/DosInfo/SpinType"][0] == "none":
-        densities = {Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"])}
-    else:
-        densities = {
-            Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"]),
-            Spin.down: np.asarray(dos["/DosInfo/Spin2/Dos"]),
-        }
-
-    efermi = dos["/DosInfo/EFermi"][0]
-
-    return Dos(efermi, energies, densities)
-
-
-def _get_total_dos_json(dos: dict) -> Dos:
-    # json -> Dos Obj
-    energies = np.asarray(dos["DosInfo"]["DosEnergy"])
-    if dos["DosInfo"]["SpinType"] == "none":
-        densities = {Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"])}
-    else:
-        densities = {
-            Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"]),
-            Spin.down: np.asarray(dos["DosInfo"]["Spin2"]["Dos"]),
-        }
-    efermi = dos["DosInfo"]["EFermi"]
-    return Dos(efermi, energies, densities)
-
-
-def _get_complete_dos(dos: dict) -> CompleteDos:
-    # h5 -> CompleteDos Obj
-    total_dos = _get_total_dos(dos)
-    structure = _get_structure(dos, "/AtomInfo")
-    N = len(structure)
-    pdos = [{} for i in range(N)]
-    number_of_spin = 1 if dos["/DosInfo/SpinType"][0] == "none" else 2
-
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-        atomindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/AtomIndexs"][0]
-        orbitindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/OrbitIndexs"][0]
-        for atom_index in range(atomindexs):
-            for orbit_index in range(orbitindexs):
-                orbit_name = Orbital(orbit_index)
-                Contribution = dos[
-                    "/DosInfo/"
-                    + spin_key
-                    + "/ProjectDos"
-                    + str(atom_index + 1)
-                    + "/"
-                    + str(orbit_index + 1)
-                ]
-                if orbit_name in pdos[atom_index].keys():
-                    pdos[atom_index][orbit_name].update({spin: Contribution})
-                else:
-                    pdos[atom_index][orbit_name] = {spin: Contribution}
-
-    pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
-
-    return CompleteDos(structure, total_dos, pdoss)
-
-
-def _get_complete_dos_json(dos: dict) -> CompleteDos:
-    # json -> CompleteDos Obj
-    total_dos = _get_total_dos_json(dos)
-    structure = _get_structure_json(dos["AtomInfo"])
-    N = len(structure)
-    pdos = [{} for i in range(N)]
-    number_of_spin = 1 if dos["DosInfo"]["SpinType"] == "none" else 2
-
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-        project = dos["DosInfo"][spin_key]["ProjectDos"]
-        for p in project:
-            atom_index = p["AtomIndex"] - 1
-            o = p["OrbitIndex"] - 1
-            orbit_name = Orbital(o)
-            if orbit_name in pdos[atom_index].keys():
-                pdos[atom_index][orbit_name].update({spin: p["Contribution"]})
-            else:
-                pdos[atom_index][orbit_name] = {spin: p["Contribution"]}
-    pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
-
-    return CompleteDos(structure, total_dos, pdoss)
-
-
-def _get_structure(hdf5: dict, key: str) -> Structure:
-    """For single-step task"""
-    # load_h5 -> Structure Obj
-    lattice = np.asarray(hdf5[key + "/Lattice"]).reshape(3, 3)
-    elements = hdf5[key + "/Elements"]
-    positions = hdf5[key + "/Position"]
-    coords = np.asarray(positions).reshape(-1, 3)
-    is_direct = hdf5[key + "/CoordinateType"][0] == "Direct"
-    elements = [re.sub(r"_", "", e) for e in elements]
-
-    return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
-
-
-def _get_structure_json(atominfo) -> Structure:
-    """For single-step task"""
-    lattice = np.asarray(atominfo["Lattice"]).reshape(3, 3)
-    elements = []
-    positions = []
-    for atom in atominfo["Atoms"]:
-        elements.append(atom["Element"])
-        positions.extend(atom["Position"])
-
-    coords = np.asarray(positions).reshape(-1, 3)
-    is_direct = atominfo["CoordinateType"] == "Direct"
-    elements = [re.sub(r"_", "", e) for e in elements]
-
-    return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
-
-
-def _get_band_data_h5(band: dict, iwan=False, zero_to_efermi=False):
-    if iwan:
-        bd = "WannBandInfo"
-    else:
-        bd = "BandInfo"
-    number_of_band = band[f"/{bd}/NumberOfBand"][0]
-    number_of_kpoints = band[f"/{bd}/NumberOfKpoints"][0]
-    if (
-        band[f"/{bd}/SpinType"][0] == "none"
-        or band[f"/{bd}/SpinType"][0] == "non-collinear"
-    ):
-        number_of_spin = 1
-    else:
-        number_of_spin = 2
-
-    symmetry_kPoints_index = band[f"/{bd}/SymmetryKPointsIndex"]
-
-    efermi = band[f"/{bd}/EFermi"][0]
-    eigenvals = {}
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-
-        if f"/{bd}/" + spin_key + "/BandEnergies" in band:
-            data = band[f"/{bd}/" + spin_key + "/BandEnergies"]
-        elif f"/{bd}/" + spin_key + "/Band" in band:
-            data = band[f"/{bd}/" + spin_key + "/Band"]
-        else:
-            print("Band key error")
-            return
-        band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-
-        if zero_to_efermi:
-            eigenvals[spin] = band_data - efermi
-            efermi = 0
-        else:
-            eigenvals[spin] = band_data
-
-    kpoints = np.asarray(band[f"/{bd}/CoordinatesOfKPoints"]).reshape(
-        number_of_kpoints, 3
-    )
-
-    structure = _get_structure(band, "/AtomInfo")
-    labels_dict = {}
-
-    for i, s in enumerate(band[f"/{bd}/SymmetryKPoints"]):
-        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
-
-    # read projection data
-    projections = None
-    if f"/{bd}/IsProject" in band.keys():
-        if band[f"/{bd}/IsProject"][0]:
-            projections = {}
-            number_of_orbit = len(band[f"/{bd}/Orbit"])
-            projection = np.zeros(
-                (number_of_band, number_of_kpoints, number_of_orbit, len(structure))
-            )
-
-            for i in range(number_of_spin):
-                spin_key = "Spin" + str(i + 1)
-                spin = Spin.up if i == 0 else Spin.down
-
-                atomindexs = band[f"/{bd}/" + spin_key + "/ProjectBand/AtomIndex"][0]
-                orbitindexs = band[f"/{bd}/" + spin_key + "/ProjectBand/OrbitIndexs"][0]
-                for atom_index in range(atomindexs):
-                    for orbit_index in range(orbitindexs):
-                        project_data = band[
-                            f"/{bd}/"
-                            + spin_key
-                            + "/ProjectBand/1/"
-                            + str(atom_index + 1)
-                            + "/"
-                            + str(orbit_index + 1)
-                        ]
-                        projection[:, :, orbit_index, atom_index] = (
-                            np.asarray(project_data)
-                            .reshape((number_of_kpoints, number_of_band))
-                            .T
-                        )
-                projections[spin] = projection
-
-    return structure, kpoints, eigenvals, efermi, labels_dict, projections
-
-
-def _get_band_data_json(
-    band: dict, syst: dict = None, iwan=False, zero_to_efermi=False
-):
-    # syst is only required for wannier band structure
-    if iwan:
-        bd = "WannBandInfo"
-        structure = _get_structure_json(syst["AtomInfo"])
-    else:
-        bd = "BandInfo"
-        structure = _get_structure_json(band["AtomInfo"])
-
-    number_of_band = band[f"{bd}"]["NumberOfBand"]
-    number_of_kpoints = band[f"{bd}"]["NumberOfKpoints"]
-    if "Spin2" in band[f"{bd}"]:
-        number_of_spin = 2
-    else:
-        number_of_spin = 1
-
-    symmetry_kPoints_index = band[f"{bd}"]["SymmetryKPointsIndex"]
-
-    if "EFermi" in band[f"{bd}"]:
-        efermi = band[f"{bd}"]["EFermi"]
-    else:
-        efermi = 0  # for wannier
-
-    eigenvals = {}
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-
-        if "BandEnergies" in band[f"{bd}"][spin_key]:
-            data = band[f"{bd}"][spin_key]["BandEnergies"]
-        elif "Band" in band[f"{bd}"][spin_key]:
-            data = band[f"{bd}"][spin_key]["Band"]
-        else:
-            print("Band key error")
-            return
-
-        band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-
-        if zero_to_efermi:
-            eigenvals[spin] = band_data - efermi
-        else:
-            eigenvals[spin] = band_data
-
-    kpoints = np.asarray(band[f"{bd}"]["CoordinatesOfKPoints"]).reshape(
-        number_of_kpoints, 3
-    )
-
-    labels_dict = {}
-
-    for i, s in enumerate(band[f"{bd}"]["SymmetryKPoints"]):
-        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
-
-    # read projection data
-    projections = None
-    if "IsProject" in band[f"{bd}"].keys():
-        if band[f"{bd}"]["IsProject"]:
-            projections = {}
-            number_of_orbit = len(band[f"{bd}"]["Orbit"])
-            projection = np.zeros(
-                (number_of_band, number_of_kpoints, number_of_orbit, len(structure))
-            )
-
-            for i in range(number_of_spin):
-                spin_key = "Spin" + str(i + 1)
-                spin = Spin.up if i == 0 else Spin.down
-
-                data = band[f"{bd}"][spin_key]["ProjectBand"]
-                for d in data:
-                    orbit_index = d["OrbitIndex"] - 1
-                    atom_index = d["AtomIndex"] - 1
-                    project_data = d["Contribution"]
-                    projection[:, :, orbit_index, atom_index] = (
-                        np.asarray(project_data)
-                        .reshape((number_of_kpoints, number_of_band))
-                        .T
-                    )
-                projections[spin] = projection
-
-    return structure, kpoints, eigenvals, efermi, labels_dict, projections
-
-
-def _get_phonon_band_data_h5(band: dict):
-    number_of_band = band["/BandInfo/NumberOfBand"][0]
-    number_of_kpoints = band["/BandInfo/NumberOfQPoints"][0]
-    number_of_spin = 1
-    symmmetry_kpoints = band["/BandInfo/SymmetryQPoints"]
-    symmetry_kPoints_index = band["/BandInfo/SymmetryQPointsIndex"]
-    eigenvals = {}
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-        if "/BandInfo/" + spin_key + "/BandEnergies" in band:
-            data = band["/BandInfo/" + spin_key + "/BandEnergies"]
-        elif "/BandInfo/" + spin_key + "/Band" in band:
-            data = band["/BandInfo/" + spin_key + "/Band"]
-        else:
-            print("Band key error")
-            return
-        frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-        eigenvals[spin] = frequencies
-    kpoints = np.asarray(band["/BandInfo/CoordinatesOfQPoints"]).reshape(
-        number_of_kpoints, 3
-    )
-    if "/SupercellAtomInfo/CoordinateType" in band.keys():
-        structure = _get_structure(band, "/SupercellAtomInfo")
-    else:
-        structure = _get_structure(band, "/AtomInfo")
-    return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
-
-
-def _get_phonon_band_data_json(band: dict):
-    number_of_band = band["BandInfo"]["NumberOfBand"]
-    number_of_kpoints = band["BandInfo"]["NumberOfQPoints"]
-    number_of_spin = 1
-    symmmetry_kpoints = band["BandInfo"]["SymmetryQPoints"]
-    symmetry_kPoints_index = band["BandInfo"]["SymmetryQPointsIndex"]
-
-    eigenvals = {}
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-        if "BandEnergies" in band["BandInfo"][spin_key]:
-            data = band["BandInfo"][spin_key]["BandEnergies"]
-        elif "Band" in band["BandInfo"][spin_key]:
-            data = band["BandInfo"][spin_key]["Band"]
-        else:
-            print("Band key error")
-            return
-        frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-        eigenvals[spin] = frequencies
-
-    kpoints = np.asarray(band["BandInfo"]["CoordinatesOfQPoints"]).reshape(
-        number_of_kpoints, 3
-    )
-
-    if "SupercellAtomInfo" in band.keys():
-        structure = _get_structure_json(band["SupercellAtomInfo"])
-    else:
-        structure = _get_structure_json(band["AtomInfo"])
-
-    return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
-
-
-def pel_from_as(spath: str, scaled=False):
-    """backup here for compatibility"""
-    with open(spath, "r") as f:
-        lines = f.readlines()
-        Natom = int(lines[1])  # 原子总数
-        ele = [line.split()[0] for line in lines[7 : 7 + Natom]]  # 元素列表
-
-        # 晶格矢量
-        latv = np.array([line.split()[0:3] for line in lines[3:6]], dtype=float)
-        # xyz坐标分量
-        coord = np.array(
-            [line.split()[1:4] for line in lines[7 : 7 + Natom]], dtype=float
-        )
-        # coordinates type
-        if lines[6].startswith("C"):  # 笛卡尔 --> 分数坐标
-            spos = np.linalg.solve(latv.T, np.transpose(coord)).T
-        elif lines[6].startswith("D"):
-            spos = coord
-        else:
-            raise ValueError(f"{spath}中的坐标类型未知！")
-
-        if scaled:
-            pos = spos
-        else:
-            pos = np.dot(spos, latv)
-
-    return pos, ele, latv
+"""
+Functions to read properties from structure or output files
+"""
+
+import json
+import os
+import re
+
+import h5py
+import numpy as np
+from pymatgen.core.lattice import Lattice
+from pymatgen.core.structure import Structure
+from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
+from pymatgen.electronic_structure.core import Orbital, Spin
+from pymatgen.electronic_structure.dos import CompleteDos, Dos
+from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine
+from pymatgen.phonon.dos import PhononDos
+
+
+def get_band_data(
+    band_dir: str,
+    syst_dir: str = None,
+    efermi: float = None,
+    zero_to_efermi: bool = False,
+) -> BandStructureSymmLine:
+    """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
+
+    Parameters
+    ----------
+    band_dir : str
+        能带文件路径，band.h5 / band.json
+    syst_dir : str
+        system.json 路径，仅为辅助处理 Wannier 数据而准备
+    efermi : float, optional
+        费米能级，如果h5文件中的费米能级不正确，可以通过此参数指定费米能级
+    zero_to_efermi : bool, optional
+        是否将费米能级移动到0
+
+    Returns
+    -------
+    BandStructureSymmLine
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_band_data
+    >>> band = get_band_data(band_dir='/data/home/hzw1002/dspawpy_repo/test/2.3/band.h5')
+
+    如果希望通过指定wannier.json来处理瓦尼尔能带，需要额外指定syst_dir参数
+
+    >>> band = get_band_data(band_dir='/data/home/hzw1002/dspawpy_repo/test/2.30/wannier.json', syst_dir='/data/home/hzw1002/dspawpy_repo/test/2.30/system.json')
+    """
+    if efermi is not None and zero_to_efermi:
+        raise ValueError(
+            "efermi and zero_to_efermi should not be set at the same time!"
+        )
+    if band_dir.endswith(".h5"):
+        band = load_h5(band_dir)
+        raw = h5py.File(band_dir, "r").keys()
+        if "/WannBandInfo/NumberOfBand" in raw:
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_h5(band, iwan=True, zero_to_efermi=zero_to_efermi)
+        elif "/BandInfo/NumberOfBand" in raw:
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_h5(band, iwan=False, zero_to_efermi=zero_to_efermi)
+        else:
+            print("BandInfo or WannBandInfo key not found in h5file!")
+            return
+    elif band_dir.endswith(".json"):
+        with open(band_dir, "r") as fin:
+            band = json.load(fin)
+        if "WannBandInfo" in band.keys():
+            assert (
+                syst_dir is not None
+            ), "system.json is required for processing wannier band info!"
+            with open(syst_dir) as system_json:
+                syst = json.load(system_json)
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_json(
+                band, syst, iwan=True, zero_to_efermi=zero_to_efermi
+            )
+        elif "BandInfo" in band.keys():
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_json(band, iwan=False, zero_to_efermi=zero_to_efermi)
+        else:
+            print("BandInfo or WannBandInfo key not found in json file!")
+            return
+    else:
+        raise TypeError(f"{os.path.abspath(band_dir)} must be h5 or json file!")
+
+    if efermi:  # 从h5直接读取的费米能级可能是错的，此时需要用户自行指定
+        rEf = efermi  # 这只是个临时解决方案
+
+    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
+    return BandStructureSymmLine(
+        kpoints=kpoints,
+        eigenvals=eigenvals,
+        lattice=lattice_new,
+        efermi=rEf,
+        labels_dict=labels_dict,
+        structure=structure,
+        projections=projections,
+    )
+
+
+def get_dos_data(dos_dir: str, return_dos=False) -> CompleteDos or Dos:
+    """读取h5或json文件中的态密度数据，构建CompleteDos或DOS对象
+
+    Parameters
+    ----------
+    dos_dir : str
+        态密度文件路径，dos.h5 / dos.json
+    return_dos : bool, optional
+        是否返回DOS对象，如果为False，则统一返回CompleteDos对象（无论计算时是否开了投影）
+
+    Returns
+    -------
+    CompleteDos or Dos
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_dos_data
+    >>> dos = get_dos_data(dos_dir='/data/home/hzw1002/dspawpy_repo/test/2.5/dos.h5')
+    """
+    if dos_dir.endswith(".h5"):
+        dos = load_h5(dos_dir)
+        if return_dos:
+            if dos["/DosInfo/Project"][0]:
+                return _get_complete_dos(dos)
+            else:
+                return _get_total_dos(dos)
+        else:
+            return _get_complete_dos(dos)
+
+    elif dos_dir.endswith(".json"):
+        with open(dos_dir, "r") as fin:
+            dos = json.load(fin)
+        if return_dos:
+            if dos["DosInfo"]["Project"]:
+                return _get_complete_dos_json(dos)
+            else:
+                return _get_total_dos_json(dos)
+        return _get_complete_dos_json(dos)
+
+    else:
+        raise TypeError(f"{os.path.abspath(dos_dir)} must be h5 or json file!")
+
+
+def get_ele_from_h5(hpath: str = "aimd.h5"):
+    """从h5文件中读取元素列表；
+    多离子步并不会在每个离子步的Structure中保存元素信息，只能读取初始结构的元素信息
+
+    Parameters
+    ----------
+    hpath : str
+        h5文件路径
+
+    Returns
+    -------
+    ele : list
+        元素列表, Natom x 1
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_ele_from_h5
+    >>> ele = get_ele_from_h5(hpath='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5')
+    >>> ele
+    ['H', 'H_1', 'O']
+    """
+    data = h5py.File(hpath)
+    Elements_bytes = np.array(data.get("/AtomInfo/Elements"))
+    tempdata = np.array([i.decode() for i in Elements_bytes])
+    ele = "".join(tempdata).split(";")
+
+    return ele
+
+
+def get_lines_without_comment(filename: str, comment: str = "#"):
+    """读取as文件内容，移除批注后返回行列表
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_lines_without_comment
+    >>> lines = get_lines_without_comment(filename='/data/home/hzw1002/dspawpy_repo/test/2.15/01/structure01.as', comment='#')
+    >>> lines
+    ['Total number of atoms', '13', 'Lattice', '5.60580000 0.00000000 0.00000000', '0.00000000 5.60580000 0.00000000', '0.00000000 0.00000000 16.81740000', 'Cartesian', 'H 2.48700709 3.85367720 6.93461994', 'Pt 1.40145000 1.40145000 1.98192999', 'Pt 4.20434996 1.40145000 1.98192999', 'Pt 1.40145000 4.20434996 1.98192999', 'Pt 4.20434996 4.20434996 1.98192999', 'Pt 0.00843706 0.00042409 3.91500875', 'Pt 0.00881029 2.80247953 3.91551673', 'Pt 2.81216310 -0.00105882 3.91807627', 'Pt 2.81156629 2.80392163 3.91572506', 'Pt 1.41398585 1.39603492 5.85554462', 'Pt 4.22886663 1.39820574 5.84677553', 'Pt 1.40485707 4.20963461 5.89521929', 'Pt 4.23788559 4.20753128 5.88625580']
+    """
+    lines = []
+    """Filter out comment lines"""
+    with open(filename) as file:
+        while True:
+            line = file.readline()
+            if line:
+                line = re.sub(comment + r".*$", "", line)  # remove comment
+                line = line.strip()
+                if line:
+                    lines.append(line)
+            else:
+                break
+
+    return lines
+
+
+def get_phonon_band_data(phonon_band_dir: str) -> PhononBandStructureSymmLine:
+    """读取h5或json文件中的声子能带数据，构建PhononBandStructureSymmLine对象
+
+    Parameters
+    ----------
+    phonon_band_dir : str
+        能带文件路径，phonon.h5 / phonon.json
+
+    Returns
+    -------
+    PhononBandStructureSymmLine
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_phonon_band_data
+    >>> band_data = get_phonon_band_data("/data/home/hzw1002/dspawpy_repo/test//2.16/phonon.h5") # 读取声子能带
+    """
+    if phonon_band_dir.endswith(".h5"):
+        band = load_h5(phonon_band_dir)
+        (
+            symmmetry_kpoints,
+            symmetry_kPoints_index,
+            kpoints,
+            structure,
+            frequencies,
+        ) = _get_phonon_band_data_h5(band)
+    elif phonon_band_dir.endswith(".json"):
+        with open(phonon_band_dir, "r") as fin:
+            band = json.load(fin)
+        (
+            symmmetry_kpoints,
+            symmetry_kPoints_index,
+            kpoints,
+            structure,
+            frequencies,
+        ) = _get_phonon_band_data_json(band)
+    else:
+        raise TypeError(f"{os.path.abspath(phonon_band_dir)} must be h5 or json file")
+
+    labels_dict = {}
+    for i, s in enumerate(symmmetry_kpoints):
+        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
+    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
+
+    return PhononBandStructureSymmLine(
+        qpoints=kpoints,
+        frequencies=frequencies,
+        lattice=lattice_new,
+        has_nac=False,
+        labels_dict=labels_dict,
+        structure=structure,
+    )
+
+
+def get_phonon_dos_data(phonon_dos_dir: str) -> PhononDos:
+    """读取h5或json文件中的声子态密度数据，构建PhononDos对象
+
+    Parameters
+    ----------
+    phonon_dos_dir : str
+        声子态密度文件路径，phonon_dos.h5 / phonon_dos.json
+
+    Returns
+    -------
+    PhononDos
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_phonon_dos_data
+    >>> phdos = get_phonon_dos_data(phonon_dos_dir='/data/home/hzw1002/dspawpy_repo/test/2.16.1/phonon.h5')
+    >>> phdos.frequencies
+    array([ 0. ,  0.1,  0.2,  0.3,  0.4,  0.5,  0.6,  0.7,  0.8,  0.9,  1. ,
+            1.1,  1.2,  1.3,  1.4,  1.5,  1.6,  1.7,  1.8,  1.9,  2. ,  2.1,
+            2.2,  2.3,  2.4,  2.5,  2.6,  2.7,  2.8,  2.9,  3. ,  3.1,  3.2,
+            3.3,  3.4,  3.5,  3.6,  3.7,  3.8,  3.9,  4. ,  4.1,  4.2,  4.3,
+            4.4,  4.5,  4.6,  4.7,  4.8,  4.9,  5. ,  5.1,  5.2,  5.3,  5.4,
+            5.5,  5.6,  5.7,  5.8,  5.9,  6. ,  6.1,  6.2,  6.3,  6.4,  6.5,
+            6.6,  6.7,  6.8,  6.9,  7. ,  7.1,  7.2,  7.3,  7.4,  7.5,  7.6,
+            7.7,  7.8,  7.9,  8. ,  8.1,  8.2,  8.3,  8.4,  8.5,  8.6,  8.7,
+            8.8,  8.9,  9. ,  9.1,  9.2,  9.3,  9.4,  9.5,  9.6,  9.7,  9.8,
+            9.9, 10. , 10.1, 10.2, 10.3, 10.4, 10.5, 10.6, 10.7, 10.8, 10.9,
+           11. , 11.1, 11.2, 11.3, 11.4, 11.5, 11.6, 11.7, 11.8, 11.9, 12. ,
+           12.1, 12.2, 12.3, 12.4, 12.5, 12.6, 12.7, 12.8, 12.9, 13. , 13.1,
+           13.2, 13.3, 13.4, 13.5, 13.6, 13.7, 13.8, 13.9, 14. , 14.1, 14.2,
+           14.3, 14.4, 14.5, 14.6, 14.7, 14.8, 14.9, 15. , 15.1, 15.2, 15.3,
+           15.4, 15.5, 15.6, 15.7, 15.8, 15.9, 16. , 16.1, 16.2, 16.3, 16.4,
+           16.5, 16.6, 16.7, 16.8, 16.9, 17. , 17.1, 17.2, 17.3, 17.4, 17.5,
+           17.6, 17.7, 17.8, 17.9, 18. , 18.1, 18.2, 18.3, 18.4, 18.5, 18.6,
+           18.7, 18.8, 18.9, 19. , 19.1, 19.2, 19.3, 19.4, 19.5, 19.6, 19.7,
+           19.8, 19.9, 20. ])
+    """
+    if phonon_dos_dir.endswith(".h5"):
+        dos = load_h5(phonon_dos_dir)
+        frequencies = np.asarray(dos["/DosInfo/DosEnergy"])
+        densities = dos["/DosInfo/Spin1/Dos"]
+    elif phonon_dos_dir.endswith(".json"):
+        with open(phonon_dos_dir, "r") as fin:
+            dos = json.load(fin)
+        frequencies = np.asarray(dos["DosInfo"]["DosEnergy"])
+        densities = dos["DosInfo"]["Spin1"]["Dos"]
+    else:
+        raise TypeError(f"{os.path.abspath(phonon_dos_dir)} must be h5 or json file")
+
+    return PhononDos(frequencies, densities)
+
+
+def get_sinfo(datafile: str, scaled=False, si=None, ele=None, ai=None):
+    r"""从datafile中读取结构信息
+
+    Parameters
+    ----------
+    datafile : str
+        h5 / json 文件路径
+    scaled : bool, optional
+        是否返回分数坐标，默认False
+    si : int or list or str, optional
+        运动轨迹中的第几步，从1开始计数！
+        如果要切片，用字符串写法： '1, 10'
+        默认为None，返回所有步
+    ele : list, optional
+        元素列表, Natom x 1
+        默认为None，从h5文件中读取
+    ai : int or list or str, optional
+        多离子步中的第几个离子步，从1开始计数
+        如果要切片，用字符串写法： '1, 10'
+        默认为None，返回所有离子步
+
+    Returns
+    -------
+    Nstep : int
+        总离子步数（几个构型）
+    ele : list
+        元素列表, Natom x 1
+    pos : np.ndarray
+        坐标分量数组，Nstep x Natom x 3
+    latv : np.ndarray
+        晶胞矢量数组，Nstep x 3 x 3
+    D_mag_fix : dict
+        磁矩、自由度相关信息
+
+    Examples
+    --------
+
+    >>> from dspawpy.io.read import get_sinfo
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='/data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5', scaled=False, si=None, ele=None, ai=None)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.18/aimd.h5...
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='/data/home/hzw1002/dspawpy_repo/test/2.1/relax.json', scaled=False, si=None, ele=None, ai=None)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.1/relax.json...
+     json所含数据默认仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！可以考虑使用io.jsonPrec参数调整精度！
+    Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info...
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='/data/home/hzw1002/dspawpy_repo/test/2.2/rho.json', scaled=False)
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.2/rho.json...
+     json所含数据默认仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！可以考虑使用io.jsonPrec参数调整精度！
+
+    这些信息可以用于进一步构建Structure对象，
+    具体参考 dspawpy.io.structure.build_Structures_from_datafile 函数
+    """
+    assert ele is None or ai is None, "不能同时选择元素和原子序号"
+
+    if datafile.endswith(".h5"):
+        assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
+        hpath = datafile
+        print(f"Reading {os.path.abspath(hpath)}...")
+        hf = h5py.File(hpath)  # 加载h5文件
+
+        # decide task type by check the internal key
+        if "/Structures" in hf.keys():  # multi-steps
+            Total_step = np.array(hf.get("/Structures/FinalStep"))[0]  # 总步数
+            if si is not None:  # 步数
+                if isinstance(si, int):  # 1
+                    indices = [si]
+
+                elif isinstance(si, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    indices = si
+
+                elif isinstance(si, str):  # ':', '-3:'
+                    indices = __parse_indices(si, Total_step)
+
+                else:
+                    raise ValueError("请输入正确格式的index")
+
+                Nstep = len(indices)
+            else:
+                Nstep = Total_step
+                indices = list(range(1, Nstep + 1))
+
+            # 读取元素列表，这个列表不会随步数改变，也不会“合并同类项”
+            Elements = np.array(get_ele_from_h5(hpath), dtype=object)
+
+            # 开始读取晶胞和原子位置
+            lattices = np.empty((Nstep, 3, 3))  # Nstep x 3 x 3
+            location = []
+            if ele is not None:  # 如果用户指定元素
+                if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
+                    ele_list = np.array(ele, dtype=object)
+                    location = np.where(Elements == ele_list)[0]
+                # 多个元素符号组成的列表，例如 ['Fe', 'O']
+                elif isinstance(ele, list) or isinstance(ele, np.ndarray):
+                    for e in ele:
+                        loc = np.where(Elements == e)[0]
+                        location.append(loc)
+                    location = np.concatenate(location)
+                else:
+                    raise TypeError("请输入正确的元素或元素列表")
+                elements = Elements[location]
+
+            elif ai is not None:  # 如果用户指定原子序号
+                if isinstance(ai, int):  # 1
+                    ais = [ai]
+                elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    ais = ai
+                elif isinstance(ai, str):  # ':', '-3:'
+                    ais = __parse_indices(ai, Total_step)
+                else:
+                    raise ValueError("请输入正确格式的ai")
+                ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
+                elements = Elements[ais]
+                location = ais
+
+            else:  # 如果都没指定
+                elements = Elements
+                location = list(range(len(Elements)))
+
+            elements = elements.tolist()  # for pretty output
+            Natom = len(elements)
+
+            poses = np.empty(shape=(len(indices), Natom, 3))
+            wrapped_poses = np.empty(shape=(len(indices), 3, Natom))
+            for i, ind in enumerate(indices):  # 步数
+                # print(f'{ind=}')
+                lats = np.array(hf.get("/Structures/Step-" + str(ind) + "/Lattice"))
+                lattices[i] = lats
+                # [x1,y1,z1,x2,y2,z2,x3,y3,z3], ...
+                # 结构优化时输出的都是分数坐标，不管CoordinateType写的是啥！
+                pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
+                wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
+                wrapped_pos = (
+                    wrapped_pos.flatten().reshape(-1, 3).T
+                )  # reshape to 3 x Natom
+                wrapped_poses[i] = wrapped_pos
+
+            iNoncollinear = False
+            try:  # 自旋计算
+                if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
+                    mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+                elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
+                    magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
+                    magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
+                    magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
+                    iNoncollinear = True
+                else:
+                    mag = np.zeros(shape=(Natom, 1))
+
+            except Exception as e:
+                if str(e):  # ignore empty AssertionError()
+                    print(e)
+                mag = np.zeros(shape=(Natom, 1))
+
+            if "/AtomInfo/Fix" in hf.keys():  # fix atom
+                atomFixs_raw = np.array(hf.get("/AtomInfo/Fix"))
+                atomFixs = np.array(
+                    ["True" if _v else "False" for _v in atomFixs_raw]
+                ).reshape(-1, 3)
+            else:
+                atomFixs = np.full(shape=(Natom, 3), fill_value="False")
+
+            try:  # fix lattice
+                latticeFixs = (
+                    np.array(hf.get("/AtomInfo/FixLattice")).astype(bool).flatten()
+                )
+                assert latticeFixs.shape == (9,)
+                latticeFixs = latticeFixs.reshape(
+                    9,
+                )  # (9,)
+            except Exception as e:
+                if str(e):  # ignore empty AssertionError()
+                    print(e)
+                latticeFixs = np.full(shape=(9,), fill_value="False")
+
+            # repeat atomFixs of shape Natom x 3 to Nstep x Natom x 3
+            atomFixs = np.repeat(atomFixs[np.newaxis, :], Nstep, axis=0).reshape(
+                Nstep, Natom, 3
+            )
+
+            # repeat latticeFixs of shape 9 x 1 to Nstep x Natom x 9
+            latticeFixs = (
+                np.repeat(latticeFixs[np.newaxis, :], Nstep * Natom, axis=0)
+                .reshape(Nstep, Natom, 9)
+                .tolist()
+            )
+
+            if iNoncollinear == False:
+                mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+                D_mag_fix = {
+                    "Mag": mags,
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+            else:
+                D_mag_fix = {
+                    "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+
+            if scaled:  # Fractional coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):  # atom si
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
+            else:  # Cartesian coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
+
+        elif "/RelaxedStructure" in hf.keys():  # 最新NEB链
+            N_images = hf.get("/RelaxedStructure").shape[0]  # Image00, Image01, ...
+            elements = np.empty(shape=(N_images,), dtype=np.float32)
+            lattices = np.empty(shape=(N_images, 3, 3), dtype=np.float32)
+            poses = np.empty(shape=(N_images, Natom, 3), dtype=np.float32)
+            atomFixs = np.empty(shape=(N_images, Natom, 3))
+            latticeFixs = np.empty(shape=(N_images, 9))
+            for i in range(N_images):
+                subfolder_name = "Image%02d" % i
+                _ele = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Elements"))[
+                    0
+                ]
+                _lat = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Lattice"))[
+                    0
+                ]
+                _pos = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Position"))[
+                    0
+                ]
+                elements[i] = _ele
+                lattices[i] = _lat
+                poses[i] = _pos
+
+                try:  # fix atom
+                    atomFix_raw = np.array(
+                        hf.get(f"/RelaxedStructure/{subfolder_name}/Fix")
+                    )
+                    atomFix = np.array(
+                        ["True" if _v else "False" for _v in atomFix_raw]
+                    ).reshape(-1, 3)
+                except:
+                    atomFix = np.full(shape=(Natom, 3), fill_value="False")
+                atomFixs[i] = atomFix
+
+                try:  # fix lattice
+                    latticeFix = (
+                        np.array(
+                            hf.get(f"/RelaxedStructure/{subfolder_name}/FixLattice")
+                        )
+                        .astype(bool)
+                        .flatten()
+                    )
+                    assert latticeFix.shape == (9,)
+                    latticeFix = latticeFix.reshape(
+                        9,
+                    )  # (9,)
+                except Exception as e:
+                    if str(e):  # ignore empty AssertionError()
+                        print(e)
+                    latticeFix = np.full(shape=(9,), fill_value="False")
+                latticeFixs[i] = latticeFix
+
+            iNoncollinear = False
+            try:  # 自旋计算
+                if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
+                    mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+                elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
+                    magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
+                    magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
+                    magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
+                    iNoncollinear = True
+                else:
+                    mag = np.zeros(shape=(Natom, 1))
+
+            except Exception as e:
+                if str(e):  # ignore empty AssertionError()
+                    print(e)
+                mag = np.zeros(shape=(Natom, 1))
+
+            if iNoncollinear == False:
+                mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+                D_mag_fix = {
+                    "Mag": mags,
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+            else:
+                D_mag_fix = {
+                    "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+
+            if scaled:  # Fractional coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):  # atom si
+                        poses[k, j, :] = np.dot(poses[k, :, sli], np.eye(3, 3))
+            else:  # Cartesian coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):
+                        poses[k, j, :] = np.dot(poses[k, :, sli], lats)
+
+        elif "/UnitAtomInfo" in hf.keys():  # phonon 仅读取单胞信息
+            hfDict = load_h5(hpath)
+            s = _get_structure(hfDict, "/UnitAtomInfo")
+            elements = s.species
+            Natom = len(elements)
+            poses = [s.cart_coords]
+            lattices = [s.lattice.matrix]
+            Nstep = 1
+
+            atomFixs = np.empty(shape=(N_images, Natom, 3))
+            atomFix = np.full(shape=(Natom, 3), fill_value="False")
+            atomFixs[0] = atomFix
+            latticeFixs = np.empty(shape=(N_images, 9))
+            latticeFix = np.full(shape=(9,), fill_value="False")
+            latticeFixs[0] = latticeFix
+
+            iNoncollinear = False
+            try:  # 自旋计算
+                if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
+                    mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+                elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
+                    magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
+                    magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
+                    magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
+                    iNoncollinear = True
+                else:
+                    mag = np.zeros(shape=(Natom, 1))
+
+            except Exception as e:
+                if str(e):  # ignore empty AssertionError()
+                    print(e)
+                mag = np.zeros(shape=(Natom, 1))
+
+            if iNoncollinear == False:
+                mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+                D_mag_fix = {
+                    "Mag": mags,
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+            else:
+                D_mag_fix = {
+                    "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+
+            if scaled:  # Fractional coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):  # atom si
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
+            else:  # Cartesian coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
+
+        else:  # rho, potential, elf, pcharge
+            hfDict = load_h5(hpath)
+            s = _get_structure(hfDict, "/AtomInfo")
+            elements = s.species
+            poses = [s.cart_coords]
+            lattices = [s.lattice.matrix]
+            Nstep = 1
+            D_mag_fix = None
+            print("--> rho/potential/elf/pcharge.h5 has no mag or fix info,")
+            print("  you should manually set it before starting new calculations..")
+
+    elif datafile.endswith(".json"):
+        assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
+        jpath = datafile
+        print(f"Reading {os.path.abspath(jpath)}...")
+        print(
+            f" json所含数据默认仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！可以考虑使用io.jsonPrec参数调整精度！"
+        )
+        with open(jpath, "r") as f:
+            data = json.load(f)  # 加载json文件
+
+        # decide the task type by checking the internal keys
+        if "AtomInfo" in data:  # single-step task
+            s = _get_structure_json(data["AtomInfo"])
+            elements = s.species
+            poses = [s.cart_coords]
+            lattices = [s.lattice.matrix]
+            Nstep = 1
+            D_mag_fix = None
+
+        elif "UnitAtomInfo" in data:  # phonon task
+            raise NotImplementedError("Read from phonon.json is not supported yet.")
+        elif "IniFin" in data:  # neb.json
+            raise NotImplementedError("Read from neb.json is not supported yet.")
+        elif "WannierInfo" in data:
+            raise NotImplementedError("wannier.json has no stucture info!")
+
+        else:  # multi-steps task
+            if "Structures" in data:
+                Total_step = len(data["Structures"])  # aimd.json
+            else:
+                Total_step = len(data)  # relax.json, neb01.json
+
+            if ele is not None and ai is not None:
+                raise ValueError("暂不支持同时指定元素和原子序号")
+            # 步数
+            if si is not None:
+                if isinstance(si, int):  # 1
+                    indices = [si]
+
+                elif isinstance(si, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    indices = si
+
+                elif isinstance(si, str):  # ':', '-3:'
+                    indices = __parse_indices(si, Total_step)
+
+                else:
+                    raise ValueError("请输入正确格式的index")
+
+                Nstep = len(indices)
+            else:
+                Nstep = Total_step
+                indices = list(range(1, Nstep + 1))  # [1,Nstep+1)
+
+            # 预先读取全部元素的总列表，这个列表不会随步数改变，也不会“合并同类项”
+            # 这样可以避免在循环内部频繁判断元素是否符合用户需要
+
+            if "Structures" in data:
+                Nele = len(data["Structures"][0]["Atoms"])  # relax.json
+                total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
+                for i in range(Nele):
+                    element = data["Structures"][0]["Atoms"][i]["Element"]
+                    total_elements[i] = element
+            else:
+                if "Atoms" not in data[0]:
+                    raise NotImplementedError("nebXX.json has no structure info!")
+                Nele = len(data[0]["Atoms"])
+                total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
+                for i in range(Nele):
+                    element = data[0]["Atoms"][i]["Element"]
+                    total_elements[i] = element
+
+            Natom = len(total_elements)
+
+            # 开始读取晶胞和原子位置
+            # 在data['Structures']['%d' % index]['Atoms']中根据元素所在序号选择结构
+            if ele is not None:  # 用户指定要某些元素
+                location = []
+                if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
+                    ele_list = list(ele)
+                # 多个元素符号组成的列表，例如 ['Fe', 'O']
+                elif isinstance(ele, list) or isinstance(ele, np.ndarray):
+                    ele_list = ele
+                else:
+                    raise TypeError("请输入正确的元素或元素列表")
+                for e in ele_list:
+                    location.append(np.where(total_elements == e)[0])
+                location = np.concatenate(location)
+
+            elif ai is not None:  # 如果用户指定原子序号，也要据此筛选元素列表
+                if isinstance(ai, int):  # 1
+                    ais = [ai]
+                elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    ais = ai
+                elif isinstance(ai, str):  # ':', '-3:'
+                    ais = __parse_indices(ai, Total_step)
+                else:
+                    raise ValueError("请输入正确格式的ai")
+                ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
+                location = ais
+                # read lattices and poses
+
+            else:  # 如果都没指定
+                location = list(range(Natom))
+
+            # 满足用户需要的elements列表
+            elements = np.empty(shape=(Natom,), dtype=object)
+            for i in range(len(location)):
+                elements[i] = total_elements[location[i]]
+
+            # Nstep x Natom x 3, positions are all fractional
+            poses = np.empty(shape=(len(indices), len(elements), 3))
+            lattices = np.empty(shape=(Nstep, 3, 3))  # Nstep x 3 x 3
+            mags = []  # Nstep x Natom x ?
+            Atomfixs = []  # Nstep x Natom x 1
+            LatFixs = []  # Nstep x Natom x 9
+
+            if "Structures" in data:  # aimd
+                for i, ind in enumerate(indices):  # for every ionic step
+                    lat = data["Structures"][ind - 1]["Lattice"]
+                    lattices[i] = np.array(lat).reshape(3, 3)
+                    mag_for_each_step = []
+                    fix_for_each_step = []
+                    if "FixLattice" in data["Structures"][ind - 1]:
+                        fixlat_raw = data["Structures"][ind - 1]["FixLattice"]
+                    else:
+                        fixlat_raw = []
+                    if fixlat_raw == []:
+                        fixlat_raw = np.full((9, 1), fill_value=False).tolist()
+                    fixlat_str = [
+                        "True" if _v == True else "False" for _v in fixlat_raw
+                    ]
+                    fixlat_arr = np.array(fixlat_str).reshape(9, 1)
+                    # repeat fixlat for each atom
+                    fixlat = np.repeat(fixlat_arr, Natom, axis=1).T.tolist()
+                    LatFixs.append(fixlat)
+                    for j, sli in enumerate(location):
+                        ati = data["Structures"][ind - 1]["Atoms"][sli]
+                        poses[i, j, :] = ati["Position"][:]
+
+                        mag_for_each_atom = ati["Mag"][:]
+                        if mag_for_each_atom == []:
+                            mag_for_each_atom = [0.0]
+                        mag_for_each_step.append(mag_for_each_atom)
+
+                        fix_for_each_atom = ati["Fix"][:]
+                        if fix_for_each_atom == []:
+                            fix_for_each_atom = ["False"]
+                        fix_for_each_step.append(fix_for_each_atom)
+
+                    mags.append(mag_for_each_step)
+                    Atomfixs.append(fix_for_each_step)
+                    if not scaled:
+                        poses[i] = np.dot(poses[i], lattices[i])
+
+            else:  # relax, neb01
+                print(
+                    "Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info..."
+                )
+
+                for i, ind in enumerate(indices):  # for every ionic step
+                    lat = data[ind - 1]["Lattice"]
+                    lattices[i] = np.array(lat).reshape(3, 3)
+                    mag_for_each_step = []
+                    fix_for_each_step = []
+                    if "FixLattice" in data[ind - 1]:
+                        fixlat_raw = data[ind - 1]["FixLattice"]
+                        if fixlat_raw == None:
+                            fixlat_raw = np.full((9, 1), fill_value=False).tolist()
+                        fixlat_str = [
+                            "True" if _v == True else "False" for _v in fixlat_raw
+                        ]
+                        fixlat_arr = np.array(fixlat_str).reshape(9, 1)
+                        # repeat fixlat for each atom
+                        fixlat = np.repeat(fixlat_arr, Natom, axis=1).T.tolist()
+                    else:
+                        fixlat = np.full((Natom, 9), fill_value=False).tolist()
+
+                    LatFixs.append(fixlat)
+                    for j, sli in enumerate(location):
+                        ati = data[ind - 1]["Atoms"][sli]
+                        poses[i, j, :] = ati["Position"][:]
+
+                        mag_for_each_atom = ati["Mag"][:]
+                        if mag_for_each_atom == []:
+                            mag_for_each_atom = [0.0]
+                        mag_for_each_step.append(mag_for_each_atom)
+
+                        fix_for_each_atom = ati["Fix"][:]
+                        if fix_for_each_atom == []:
+                            fix_for_each_atom = ["False"]
+                        fix_for_each_step.append(fix_for_each_atom)
+
+                    mags.append(mag_for_each_step)
+                    Atomfixs.append(fix_for_each_step)
+                    if not scaled:
+                        poses[i] = np.dot(poses[i], lattices[i])
+
+            elements = elements.tolist()
+            Mags = np.array(mags).tolist()  # (Nstep, Natom, ?) or (Nstep, 0,)
+
+            D_mag_fix = {"Mag": Mags, "Fix": Atomfixs, "LatticeFixs": LatFixs}
+
+    else:
+        raise ValueError(
+            "get_sinfo function only accept datafile of .h5 / .json format!"
+        )
+
+    return Nstep, elements, poses, lattices, D_mag_fix
+
+
+def load_h5(dir_h5: str) -> dict:
+    """遍历读取h5文件中的数据，保存为字典格式
+
+    慎用此函数，因为会读取很多不需要的数据，耗时很长。
+
+    Parameters
+    ----------
+    dir_h5 : str
+        h5文件路径
+
+    Returns
+    -------
+    datas: dict
+        数据字典
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import load_h5
+    >>> datas = load_h5(dir_h5='/data/home/hzw1002/dspawpy_repo/test/2.2/scf.h5')
+    >>> datas.keys()
+    dict_keys(['/AtomInfo/CoordinateType', '/AtomInfo/Elements', '/AtomInfo/Grid', '/AtomInfo/Lattice', '/AtomInfo/Position', '/Eigenvalue/CBM/BandIndex', '/Eigenvalue/CBM/Energy', '/Eigenvalue/CBM/Kpoint', '/Eigenvalue/NumberOfBand', '/Eigenvalue/Spin1/BandEnergies', '/Eigenvalue/Spin1/Kpoints/Coordinates', '/Eigenvalue/Spin1/Kpoints/Grid', '/Eigenvalue/Spin1/Kpoints/NumberOfKpoints', '/Eigenvalue/Spin1/Occupation', '/Eigenvalue/VBM/BandIndex', '/Eigenvalue/VBM/Energy', '/Eigenvalue/VBM/Kpoint', '/Electron', '/Energy/EFermi', '/Energy/TotalEnergy', '/Energy/TotalEnergy0', '/Force/ForceOnAtoms', '/Stress/Direction', '/Stress/Pressure', '/Stress/Stress', '/Stress/Total', '/Structures/FinalStep', '/Structures/Step-1/Lattice', '/Structures/Step-1/Position'])
+    """
+
+    def get_names(key, h5_object):
+        names.append(h5_object.name)
+
+    def is_dataset(name):
+        for name_inTheList in names:
+            if name_inTheList.find(name + "/") != -1:
+                return False
+        return True
+
+    def get_datas(key, h5_object):
+        if is_dataset(h5_object.name):
+            data = np.asarray(h5_object)
+            if data.dtype == "|S1":  # 转成字符串 并根据";"分割
+                byte2str = [str(bi, "utf-8") for bi in data]
+                string = ""
+                for char in byte2str:
+                    string += char
+                data = np.array([elem for elem in string.strip().split(";")])
+            # "/group1/group2/.../groupN/dataset" : value
+            datas[h5_object.name] = data.tolist()
+
+    with h5py.File(dir_h5, "r") as fin:
+        names = []
+        datas = {}
+        fin.visititems(get_names)
+        fin.visititems(get_datas)
+
+        return datas
+
+
+def load_h5_todict(dir_h5: str) -> dict:
+    """与上一个函数区别在于合并了部分同类数据，例如
+
+    /Structures/Step-1/* 和 /Structures/Step-2/* 并入 /Structures/ 组内
+    """
+
+    def create_dict(L: list, D: dict):
+        if len(L) == 2:
+            D[L[0]] = L[1]
+            return
+        else:
+            if not (L[0] in D.keys()):
+                D[L[0]] = {}
+            create_dict(L[1:], D[L[0]])
+
+    datas = load_h5(dir_h5)
+
+    groups_value_list = []
+    for key in datas.keys():
+        tmp_list = key[1:].strip().split("/")  # [1:] 截去root
+        tmp_list.append(datas[key])
+        # groups_value_list[i]结构: [group1, group2, ..., groupN, dataset, value]
+        groups_value_list.append(tmp_list)
+
+    groups_value_dict = {}
+    for data in groups_value_list:
+        create_dict(data, groups_value_dict)
+
+    return groups_value_dict
+
+
+def __parse_indices(index: str, total_step) -> list:
+    """解析用户输入的原子序号字符串
+
+    输入：
+        - index: 用户输入的原子序号/元素字符串，例如 '1:3,5,7:10'
+    输出：
+        - indices: 解析后的原子序号列表，例如 [1,2,3,4,5,6,7,8,9,10]
+    """
+    assert ":" in index, "如果不想切片索引，请输入整数或者列表"
+    blcs = index.split(",")
+    indices = []
+    for blc in blcs:
+        if ":" in blc:  # 切片
+            low = blc.split(":")[0]
+            if not low:
+                low = 1  # 从1开始
+            else:
+                low = int(low)
+                assert low > 0, "索引从1开始！"
+            high = blc.split(":")[1]
+            if not high:
+                high = total_step
+            else:
+                high = int(high)
+                assert high <= total_step, "索引超出范围！"
+
+            for i in range(low, high + 1):
+                indices.append(i)
+        else:  # 单个数字
+            indices.append(int(blc))
+    return indices
+
+
+def _get_lammps_non_orthogonal_box(lat: np.ndarray):
+    """计算用于输入lammps的盒子边界参数，用于生成dump结构文件
+
+    Parameters
+    ----------
+    lat : np.ndarray
+        常见的非三角3x3矩阵
+
+    Returns
+    -------
+    box_bounds:
+        用于输入lammps的盒子边界
+    """
+    # https://docs.lammps.org/Howto_triclinic.html
+    A = lat[0]
+    B = lat[1]
+    C = lat[2]
+    assert np.cross(A, B).dot(C) > 0, "Lat is not right handed"
+
+    # 将常规3x3矩阵转成标准的上三角矩阵
+    alpha = np.arccos(np.dot(B, C) / (np.linalg.norm(B) * np.linalg.norm(C)))
+    beta = np.arccos(np.dot(A, C) / (np.linalg.norm(A) * np.linalg.norm(C)))
+    gamma = np.arccos(np.dot(A, B) / (np.linalg.norm(A) * np.linalg.norm(B)))
+
+    ax = np.linalg.norm(A)
+    a = np.array([ax, 0, 0])
+
+    bx = np.linalg.norm(B) * np.cos(gamma)
+    by = np.linalg.norm(B) * np.sin(gamma)
+    b = np.array([bx, by, 0])
+
+    cx = np.linalg.norm(C) * np.cos(beta)
+    cy = (np.linalg.norm(B) * np.linalg.norm(C) - bx * cx) / by
+    cz = np.sqrt(abs(np.linalg.norm(C) ** 2 - cx**2 - cy**2))
+    c = np.array([cx, cy, cz])
+
+    # triangluar matrix in lammmps cell format
+    # note that in OVITO, it will be down-triangular one
+    # lammps_lattice = np.array([a,b,c]).T
+
+    # write lammps box parameters
+    # https://docs.lammps.org/Howto_triclinic.html#:~:text=The%20inverse%20relationship%20can%20be%20written%20as%20follows
+    lx = np.linalg.norm(a)
+    xy = np.linalg.norm(b) * np.cos(gamma)
+    xz = np.linalg.norm(c) * np.cos(beta)
+    ly = np.sqrt(np.linalg.norm(b) ** 2 - xy**2)
+    yz = (np.linalg.norm(b) * np.linalg.norm(c) * np.cos(alpha) - xy * xz) / ly
+    lz = np.sqrt(np.linalg.norm(c) ** 2 - xz**2 - yz**2)
+
+    # "The parallelepiped has its “origin” at (xlo,ylo,zlo) and is defined by 3 edge vectors starting from the origin given by a = (xhi-xlo,0,0); b = (xy,yhi-ylo,0); c = (xz,yz,zhi-zlo)."
+    # 令原点在(0,0,0)，则 xlo = ylo = zlo = 0
+    xlo = ylo = zlo = 0
+    # https://docs.lammps.org/Howto_triclinic.html#:~:text=the%20LAMMPS%20box%20sizes%20(lx%2Cly%2Clz)%20%3D%20(xhi%2Dxlo%2Cyhi%2Dylo%2Czhi%2Dzlo)
+    xhi = lx + xlo
+    yhi = ly + ylo
+    zhi = lz + zlo
+    # https://docs.lammps.org/Howto_triclinic.html#:~:text=This%20bounding%20box%20is%20convenient%20for%20many%20visualization%20programs%20and%20is%20calculated%20from%20the%209%20triclinic%20box%20parameters%20(xlo%2Cxhi%2Cylo%2Cyhi%2Czlo%2Czhi%2Cxy%2Cxz%2Cyz)%20as%20follows%3A
+    xlo_bound = xlo + np.min([0, xy, xz, xy + xz])
+    xhi_bound = xhi + np.max([0, xy, xz, xy + xz])
+    ylo_bound = ylo + np.min([0, yz])
+    yhi_bound = yhi + np.max([0, yz])
+    zlo_bound = zlo
+    zhi_bound = zhi
+    box_bounds = np.array(
+        [
+            [xlo_bound, xhi_bound, xy],
+            [ylo_bound, yhi_bound, xz],
+            [zlo_bound, zhi_bound, yz],
+        ]
+    )
+
+    return box_bounds
+
+
+def _get_total_dos(dos: dict) -> Dos:
+    # h5 -> Dos Obj
+    energies = np.asarray(dos["/DosInfo/DosEnergy"])
+    if dos["/DosInfo/SpinType"][0] == "none":
+        densities = {Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"])}
+    else:
+        densities = {
+            Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"]),
+            Spin.down: np.asarray(dos["/DosInfo/Spin2/Dos"]),
+        }
+
+    efermi = dos["/DosInfo/EFermi"][0]
+
+    return Dos(efermi, energies, densities)
+
+
+def _get_total_dos_json(dos: dict) -> Dos:
+    # json -> Dos Obj
+    energies = np.asarray(dos["DosInfo"]["DosEnergy"])
+    if dos["DosInfo"]["SpinType"] == "none":
+        densities = {Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"])}
+    else:
+        densities = {
+            Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"]),
+            Spin.down: np.asarray(dos["DosInfo"]["Spin2"]["Dos"]),
+        }
+    efermi = dos["DosInfo"]["EFermi"]
+    return Dos(efermi, energies, densities)
+
+
+def _get_complete_dos(dos: dict) -> CompleteDos:
+    # h5 -> CompleteDos Obj
+    total_dos = _get_total_dos(dos)
+    structure = _get_structure(dos, "/AtomInfo")
+    N = len(structure)
+    pdos = [{} for i in range(N)]
+    number_of_spin = 1 if dos["/DosInfo/SpinType"][0] == "none" else 2
+
+    if dos["/DosInfo/Project"][0] == 0:  # not project dos
+        pdoss = None
+    else:
+        for i in range(number_of_spin):
+            spin_key = "Spin" + str(i + 1)
+            spin = Spin.up if i == 0 else Spin.down
+            atomindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/AtomIndexs"][0]
+            orbitindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/OrbitIndexs"][0]
+            for atom_index in range(atomindexs):
+                for orbit_index in range(orbitindexs):
+                    orbit_name = Orbital(orbit_index)
+                    Contribution = dos[
+                        "/DosInfo/"
+                        + spin_key
+                        + "/ProjectDos"
+                        + str(atom_index + 1)
+                        + "/"
+                        + str(orbit_index + 1)
+                    ]
+                    if orbit_name in pdos[atom_index].keys():
+                        pdos[atom_index][orbit_name].update({spin: Contribution})
+                    else:
+                        pdos[atom_index][orbit_name] = {spin: Contribution}
+
+        pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
+
+    return CompleteDos(structure, total_dos, pdoss)
+
+
+def _get_complete_dos_json(dos: dict) -> CompleteDos:
+    # json -> CompleteDos Obj
+    total_dos = _get_total_dos_json(dos)
+    structure = _get_structure_json(dos["AtomInfo"])
+    N = len(structure)
+    pdos = [{} for i in range(N)]
+    number_of_spin = 1 if dos["DosInfo"]["SpinType"] == "none" else 2
+
+    if dos["DosInfo"]["Project"] == False:  # not project dos
+        pdoss = None
+    else:
+        for i in range(number_of_spin):
+            spin_key = "Spin" + str(i + 1)
+            spin = Spin.up if i == 0 else Spin.down
+            project = dos["DosInfo"][spin_key]["ProjectDos"]
+            for p in project:
+                atom_index = p["AtomIndex"] - 1
+                o = p["OrbitIndex"] - 1
+                orbit_name = Orbital(o)
+                if orbit_name in pdos[atom_index].keys():
+                    pdos[atom_index][orbit_name].update({spin: p["Contribution"]})
+                else:
+                    pdos[atom_index][orbit_name] = {spin: p["Contribution"]}
+        pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
+
+    return CompleteDos(structure, total_dos, pdoss)
+
+
+def _get_structure(hdf5: dict, key: str) -> Structure:
+    """For single-step task"""
+    # load_h5 -> Structure Obj
+    lattice = np.asarray(hdf5[key + "/Lattice"]).reshape(3, 3)
+    elements = hdf5[key + "/Elements"]
+    positions = hdf5[key + "/Position"]
+    coords = np.asarray(positions).reshape(-1, 3)
+    is_direct = hdf5[key + "/CoordinateType"][0] == "Direct"
+    elements = [re.sub(r"_", "", e) for e in elements]
+
+    return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
+
+
+def _get_structure_json(atominfo) -> Structure:
+    """For single-step task"""
+    lattice = np.asarray(atominfo["Lattice"]).reshape(3, 3)
+    elements = []
+    positions = []
+    for atom in atominfo["Atoms"]:
+        elements.append(atom["Element"])
+        positions.extend(atom["Position"])
+
+    coords = np.asarray(positions).reshape(-1, 3)
+    is_direct = atominfo["CoordinateType"] == "Direct"
+    elements = [re.sub(r"_", "", e) for e in elements]
+
+    return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
+
+
+def _get_band_data_h5(band: dict, iwan=False, zero_to_efermi=False):
+    if iwan:
+        bd = "WannBandInfo"
+    else:
+        bd = "BandInfo"
+    number_of_band = band[f"/{bd}/NumberOfBand"][0]
+    number_of_kpoints = band[f"/{bd}/NumberOfKpoints"][0]
+    if (
+        band[f"/{bd}/SpinType"][0] == "none"
+        or band[f"/{bd}/SpinType"][0] == "non-collinear"
+    ):
+        number_of_spin = 1
+    else:
+        number_of_spin = 2
+
+    symmetry_kPoints_index = band[f"/{bd}/SymmetryKPointsIndex"]
+
+    efermi = band[f"/{bd}/EFermi"][0]
+    eigenvals = {}
+    for i in range(number_of_spin):
+        spin_key = "Spin" + str(i + 1)
+        spin = Spin.up if i == 0 else Spin.down
+
+        if f"/{bd}/" + spin_key + "/BandEnergies" in band:
+            data = band[f"/{bd}/" + spin_key + "/BandEnergies"]
+        elif f"/{bd}/" + spin_key + "/Band" in band:
+            data = band[f"/{bd}/" + spin_key + "/Band"]
+        else:
+            print("Band key error")
+            return
+        band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
+
+        if zero_to_efermi:
+            eigenvals[spin] = band_data - efermi
+            efermi = 0
+        else:
+            eigenvals[spin] = band_data
+
+    kpoints = np.asarray(band[f"/{bd}/CoordinatesOfKPoints"]).reshape(
+        number_of_kpoints, 3
+    )
+
+    structure = _get_structure(band, "/AtomInfo")
+    labels_dict = {}
+
+    for i, s in enumerate(band[f"/{bd}/SymmetryKPoints"]):
+        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
+
+    # read projection data
+    projections = None
+    if f"/{bd}/IsProject" in band.keys():
+        if band[f"/{bd}/IsProject"][0]:
+            projections = {}
+            number_of_orbit = len(band[f"/{bd}/Orbit"])
+            projection = np.zeros(
+                (number_of_band, number_of_kpoints, number_of_orbit, len(structure))
+            )
+
+            for i in range(number_of_spin):
+                spin_key = "Spin" + str(i + 1)
+                spin = Spin.up if i == 0 else Spin.down
+
+                atomindexs = band[f"/{bd}/" + spin_key + "/ProjectBand/AtomIndex"][0]
+                orbitindexs = band[f"/{bd}/" + spin_key + "/ProjectBand/OrbitIndexs"][0]
+                for atom_index in range(atomindexs):
+                    for orbit_index in range(orbitindexs):
+                        project_data = band[
+                            f"/{bd}/"
+                            + spin_key
+                            + "/ProjectBand/1/"
+                            + str(atom_index + 1)
+                            + "/"
+                            + str(orbit_index + 1)
+                        ]
+                        projection[:, :, orbit_index, atom_index] = (
+                            np.asarray(project_data)
+                            .reshape((number_of_kpoints, number_of_band))
+                            .T
+                        )
+                projections[spin] = projection
+
+    return structure, kpoints, eigenvals, efermi, labels_dict, projections
+
+
+def _get_band_data_json(
+    band: dict, syst: dict = None, iwan=False, zero_to_efermi=False
+):
+    # syst is only required for wannier band structure
+    if iwan:
+        bd = "WannBandInfo"
+        structure = _get_structure_json(syst["AtomInfo"])
+    else:
+        bd = "BandInfo"
+        structure = _get_structure_json(band["AtomInfo"])
+
+    number_of_band = band[f"{bd}"]["NumberOfBand"]
+    number_of_kpoints = band[f"{bd}"]["NumberOfKpoints"]
+    if "Spin2" in band[f"{bd}"]:
+        number_of_spin = 2
+    else:
+        number_of_spin = 1
+
+    symmetry_kPoints_index = band[f"{bd}"]["SymmetryKPointsIndex"]
+
+    if "EFermi" in band[f"{bd}"]:
+        efermi = band[f"{bd}"]["EFermi"]
+    else:
+        efermi = 0  # for wannier
+
+    eigenvals = {}
+    for i in range(number_of_spin):
+        spin_key = "Spin" + str(i + 1)
+        spin = Spin.up if i == 0 else Spin.down
+
+        if "BandEnergies" in band[f"{bd}"][spin_key]:
+            data = band[f"{bd}"][spin_key]["BandEnergies"]
+        elif "Band" in band[f"{bd}"][spin_key]:
+            data = band[f"{bd}"][spin_key]["Band"]
+        else:
+            print("Band key error")
+            return
+
+        band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
+
+        if zero_to_efermi:
+            eigenvals[spin] = band_data - efermi
+            efermi = 0
+        else:
+            eigenvals[spin] = band_data
+
+    kpoints = np.asarray(band[f"{bd}"]["CoordinatesOfKPoints"]).reshape(
+        number_of_kpoints, 3
+    )
+
+    labels_dict = {}
+
+    for i, s in enumerate(band[f"{bd}"]["SymmetryKPoints"]):
+        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
+
+    # read projection data
+    projections = None
+    if "IsProject" in band[f"{bd}"].keys():
+        if band[f"{bd}"]["IsProject"]:
+            projections = {}
+            number_of_orbit = len(band[f"{bd}"]["Orbit"])
+            projection = np.zeros(
+                (number_of_band, number_of_kpoints, number_of_orbit, len(structure))
+            )
+
+            for i in range(number_of_spin):
+                spin_key = "Spin" + str(i + 1)
+                spin = Spin.up if i == 0 else Spin.down
+
+                data = band[f"{bd}"][spin_key]["ProjectBand"]
+                for d in data:
+                    orbit_index = d["OrbitIndex"] - 1
+                    atom_index = d["AtomIndex"] - 1
+                    project_data = d["Contribution"]
+                    projection[:, :, orbit_index, atom_index] = (
+                        np.asarray(project_data)
+                        .reshape((number_of_kpoints, number_of_band))
+                        .T
+                    )
+                projections[spin] = projection
+
+    return structure, kpoints, eigenvals, efermi, labels_dict, projections
+
+
+def _get_phonon_band_data_h5(band: dict):
+    number_of_band = band["/BandInfo/NumberOfBand"][0]
+    number_of_kpoints = band["/BandInfo/NumberOfQPoints"][0]
+    number_of_spin = 1
+    symmmetry_kpoints = band["/BandInfo/SymmetryQPoints"]
+    symmetry_kPoints_index = band["/BandInfo/SymmetryQPointsIndex"]
+    eigenvals = {}
+    for i in range(number_of_spin):
+        spin_key = "Spin" + str(i + 1)
+        spin = Spin.up if i == 0 else Spin.down
+        if "/BandInfo/" + spin_key + "/BandEnergies" in band:
+            data = band["/BandInfo/" + spin_key + "/BandEnergies"]
+        elif "/BandInfo/" + spin_key + "/Band" in band:
+            data = band["/BandInfo/" + spin_key + "/Band"]
+        else:
+            print("Band key error")
+            return
+        frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
+        eigenvals[spin] = frequencies
+    kpoints = np.asarray(band["/BandInfo/CoordinatesOfQPoints"]).reshape(
+        number_of_kpoints, 3
+    )
+    if "/SupercellAtomInfo/CoordinateType" in band.keys():
+        structure = _get_structure(band, "/SupercellAtomInfo")
+    else:
+        structure = _get_structure(band, "/AtomInfo")
+    return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
+
+
+def _get_phonon_band_data_json(band: dict):
+    number_of_band = band["BandInfo"]["NumberOfBand"]
+    number_of_kpoints = band["BandInfo"]["NumberOfQPoints"]
+    number_of_spin = 1
+    symmmetry_kpoints = band["BandInfo"]["SymmetryQPoints"]
+    symmetry_kPoints_index = band["BandInfo"]["SymmetryQPointsIndex"]
+
+    eigenvals = {}
+    for i in range(number_of_spin):
+        spin_key = "Spin" + str(i + 1)
+        spin = Spin.up if i == 0 else Spin.down
+        if "BandEnergies" in band["BandInfo"][spin_key]:
+            data = band["BandInfo"][spin_key]["BandEnergies"]
+        elif "Band" in band["BandInfo"][spin_key]:
+            data = band["BandInfo"][spin_key]["Band"]
+        else:
+            print("Band key error")
+            return
+        frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
+        eigenvals[spin] = frequencies
+
+    kpoints = np.asarray(band["BandInfo"]["CoordinatesOfQPoints"]).reshape(
+        number_of_kpoints, 3
+    )
+
+    if "SupercellAtomInfo" in band.keys():
+        structure = _get_structure_json(band["SupercellAtomInfo"])
+    else:
+        structure = _get_structure_json(band["AtomInfo"])
+
+    return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
+
+
+def pel_from_as(spath: str, scaled=False):
+    """backup here for compatibility"""
+    with open(spath, "r") as f:
+        lines = f.readlines()
+        Natom = int(lines[1])  # 原子总数
+        ele = [line.split()[0] for line in lines[7 : 7 + Natom]]  # 元素列表
+
+        # 晶格矢量
+        latv = np.array([line.split()[0:3] for line in lines[3:6]], dtype=float)
+        # xyz坐标分量
+        coord = np.array(
+            [line.split()[1:4] for line in lines[7 : 7 + Natom]], dtype=float
+        )
+        # coordinates type
+        if lines[6].startswith("C"):  # 笛卡尔 --> 分数坐标
+            spos = np.linalg.solve(latv.T, np.transpose(coord)).T
+        elif lines[6].startswith("D"):
+            spos = coord
+        else:
+            raise ValueError(f"{spath}中的坐标类型未知！")
+
+        if scaled:
+            pos = spos
+        else:
+            pos = np.dot(spos, latv)
+
+    return pos, ele, latv
+
+
+def _remove_extra_kpoint(band_data, symmetry_kPoints_index, number_of_band):
+    keep_data = []
+    for i in range(len(symmetry_kPoints_index) - 1):
+        if i == 0:
+            start_index = symmetry_kPoints_index[i] - 1
+            end_index = symmetry_kPoints_index[i + 1]
+        else:
+            start_index = symmetry_kPoints_index[i] + 1
+            end_index = symmetry_kPoints_index[i + 1]
+
+        tmp = band_data[start_index * number_of_band : end_index * number_of_band]
+        keep_data.extend(tmp)
+    return keep_data
```

## dspawpy/io/structure.py

```diff
@@ -1,295 +1,299 @@
-"""
-Functions to build structures
-"""
-
-import re
-from typing import List, Union
-
-import numpy as np
-from pymatgen.core import Structure
-
-from dspawpy.io.read import get_lines_without_comment, get_sinfo
-
-
-def build_Structures_from_datafile(
-    datafile: Union[str, List[str]], si=None, ele=None, ai=None, fmt=None
-) -> List[Structure]:
-    r"""读取一/多个h5/json文件，返回pymatgen的Structures列表
-
-    Parameters
-    ----------
-    datafile : str or list
-        - h5/json/as/hzw/cif/poscar/cssr/xsf/mcsqs/prismatic/yaml/fleur-inpgen文件路径;
-        - 若给定字符串列表，将依次读取数据并合并成一个Structures列表
-        - 文件类型依据后缀名判断，请勿使用不规范的后缀名
-    si: int, list or str
-        构型编号，从 1 开始
-        - si=1, 读取第一个构型
-        - si=[1,2], 读取第一个和第二个构型
-        - si=':', 读取所有构型
-        - si='-3:', 读取最后三个构型
-    ele: str or list
-        元素符号，如['H','O']
-    ai: int or list
-        原子编号，从 1 开始，用法同si
-    fmt: str
-        文件格式，包括 'h5', 'json', 'as', 'hzw' 四种，其他值将被忽略。详见 http://hzwtech.com/Device%20Studio/DS-PAW/build/html/tools.html#structure 8.2节表格
-
-
-    Returns
-    -------
-    List[Structure] : pymatgen Structures 列表
-
-    Examples
-    --------
-
-    >>> from dspawpy.io.structure import build_Structures_from_datafile
-
-    读取单个文件生成 Structures 列表，支持四种类型
-
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='/data/home/hzw1002/dspawpy_repo/test/2.1/relax.h5')
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.1/relax.h5...
-    >>> len(pymatgen_Structures)
-    3
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='/data/home/hzw1002/dspawpy_repo/test/2.1/relax.json')
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.1/relax.json...
-     json所含数据仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！
-    Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info...
-    >>> len(pymatgen_Structures)
-    3
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='/data/home/hzw1002/dspawpy_repo/test/supplement/PtH.as')
-    >>> len(pymatgen_Structures)
-    1
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='/data/home/hzw1002/dspawpy_repo/test/supplement/PtH.hzw')
-    build from hzw file may lack mag & fix info!
-    >>> len(pymatgen_Structures)
-    1
-
-    注意pymatgen_Structures是由多个 Structure 对象组成的列表，每个 Structure 对象分别对应一个构型。如果只有一个构型，也会返回列表，请使用 pymatgen_Structures[0] 获取 Structure 对象
-
-    当datafile为列表时，将依次读取多个文件，合并成一个Structures列表
-
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile=['/data/home/hzw1002/dspawpy_repo/test/supplement/aimd1.h5','/data/home/hzw1002/dspawpy_repo/test/supplement/aimd2.h5'])
-    Reading /data/home/hzw1002/dspawpy_repo/test/supplement/aimd1.h5...
-    Reading /data/home/hzw1002/dspawpy_repo/test/supplement/aimd2.h5...
-    """
-    dfs = []
-    if isinstance(datafile, list):  # 续算模式，给的是多个文件
-        dfs = datafile
-    else:  # 单次计算模式，处理单个文件
-        dfs.append(datafile)
-
-    # 读取结构数据
-    pymatgen_Structures = []
-    for df in dfs:
-        structure_list = _get_structure_list(df, si, ele, ai, fmt)
-        pymatgen_Structures.extend(structure_list)
-
-    return pymatgen_Structures
-
-
-def _get_structure_list(
-    df: str, si=None, ele=None, ai=None, fmt=None
-) -> List[Structure]:
-    """get pymatgen structures from single datafile
-
-    Parameters
-    ----------
-    df : str
-        datafile
-
-    Returns
-    -------
-    List[Structure] : list of pymatgen structures
-    """
-
-    if fmt is None:
-        fmt = df.split(".")[-1]
-    else:
-        assert isinstance(fmt, str), "fmt must be str"
-
-    if fmt == "as":
-        strs = [_from_dspaw_as(df)]
-    elif fmt == "hzw":
-        print("build from hzw file may lack mag & fix info!")
-        strs = [_from_hzw(df)]
-    elif fmt == "h5" or fmt == "json":
-        Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
-            datafile=df, si=si, ele=ele, ai=ai
-        )  # returned positions, not scaled-positions
-        # remove _ from elements
-        elements = [re.sub(r"_", "", e) for e in elements]
-
-        strs = []
-        for i in range(Nstep):
-            if D_mag_fix:
-                strs.append(
-                    Structure(
-                        lattices[i],
-                        elements,
-                        positions[i],
-                        coords_are_cartesian=True,
-                        site_properties={k: v[i] for k, v in D_mag_fix.items()},
-                    )
-                )
-            else:
-                strs.append(
-                    Structure(
-                        lattices[i],
-                        elements,
-                        positions[i],
-                        coords_are_cartesian=True,
-                    )
-                )
-    else:
-        strs = [Structure.from_file(df)]
-
-    return strs
-
-
-def _from_dspaw_as(as_file: str = "structure.as") -> Structure:
-    """从DSPAW的as结构文件中读取结构信息
-
-    Parameters
-    ----------
-    as_file : str
-        DSPAW的as结构文件, 默认'structure.as'
-
-    Returns
-    -------
-    Structure
-        pymatgen的Structure对象
-    """
-
-    lines = get_lines_without_comment(as_file, "#")
-    N = int(lines[1])  # number of atoms
-
-    # parse lattice info
-    lattice = []  # lattice matrix
-    for line in lines[3:6]:
-        vector = line.split()
-        lattice.extend([float(vector[0]), float(vector[1]), float(vector[2])])
-    lattice = np.asarray(lattice).reshape(3, 3)
-
-    lat_fixs = []
-    if lines[2].strip() != "Lattice":  # fix lattice
-        lattice_fix_info = lines[2].strip().split()[1:]
-        if lattice_fix_info == ["Fix_x", "Fix_y", "Fix_z"]:
-            # ONLY support xyz fix in sequence, yzx will cause error
-            for line in lines[3:6]:
-                lfs = line.strip().split()[3:6]
-                for lf in lfs:
-                    if lf.startswith("T"):
-                        lat_fixs.append("True")
-                    elif lf.startswith("F"):
-                        lat_fixs.append("False")
-        elif lattice_fix_info == ["Fix"]:
-            for line in lines[3:6]:
-                lf = line.strip().split()[3]
-                if lf.startswith("T"):
-                    lat_fixs.append("True")
-                elif lf.startswith("F"):
-                    lat_fixs.append("False")
-        else:
-            raise ValueError("Lattice fix info error!")
-
-    elements = []
-    positions = []
-    for i in range(N):
-        atom = lines[i + 7].strip().split()
-        elements.append(atom[0])
-        positions.extend([float(atom[1]), float(atom[2]), float(atom[3])])
-
-    mf_info = None
-    l6 = lines[6].strip()  # str, 'Cartesian/Direct Mag Fix_x ...'
-    if l6 == "Direct":
-        is_direct = True
-    elif l6 == "Cartesian":
-        is_direct = False
-    else:
-        is_direct = l6.split()[0] == "Direct"
-        mf_info = l6.split()[1:]  # ['Mag', 'Fix_x', 'Fix_y', 'Fix_z']
-        for item in mf_info:
-            assert item in [
-                "Mag",
-                "Mag_x",
-                "Mag_y",
-                "Mag_z",
-                "Fix",
-                "Fix_x",
-                "Fix_y",
-                "Fix_z",
-            ], "Mag/Fix info error!"
-
-    mag_fix_dict = {}
-    if mf_info is not None:
-        for mf_index, item in enumerate(mf_info):
-            values = []
-            for i in range(N):
-                atom = lines[i + 7].strip().split()
-                mf = atom[4:]
-                values.append(mf[mf_index])
-
-            if item.startswith("Fix"):  # F -> False, T -> True
-                for value in values:
-                    if value.startswith("T"):
-                        values[values.index(value)] = "True"
-                    elif value.startswith("F"):
-                        values[values.index(value)] = "False"
-            mag_fix_dict[item] = values
-
-    if lat_fixs != []:
-        # replicate lat_fixs to N atoms
-        mag_fix_dict["LatticeFixs"] = [lat_fixs for i in range(N)]
-
-    coords = np.asarray(positions).reshape(-1, 3)
-    # remove _ from elements
-    elements = [re.sub(r"_", "", e) for e in elements]
-
-    if mag_fix_dict == {}:
-        return Structure(
-            lattice, elements, coords, coords_are_cartesian=(not is_direct)
-        )
-    else:
-        return Structure(
-            lattice,
-            elements,
-            coords,
-            coords_are_cartesian=(not is_direct),
-            site_properties=mag_fix_dict,
-        )
-
-
-def _from_hzw(hzw_file) -> Structure:
-    """从hzw结构文件中读取结构信息
-
-    Parameters
-    ----------
-    hzw_file : str
-        hzw结构文件，以 .hzw 结尾
-
-    Returns
-    -------
-    Structure
-        pymatgen的Structure对象
-    """
-    lines = get_lines_without_comment(hzw_file, "%")
-    number_of_probes = int(lines[0])
-    if number_of_probes != 0:
-        raise ValueError("dspaw only support 0 probes hzw file")
-    lattice = []
-    for line in lines[1:4]:
-        vector = line.split()
-        lattice.extend([float(vector[0]), float(vector[1]), float(vector[2])])
-
-    lattice = np.asarray(lattice).reshape(3, 3)
-    N = int(lines[4])
-    elements = []
-    positions = []
-    for i in range(N):
-        atom = lines[i + 5].strip().split()
-        elements.append(atom[0])
-        positions.extend([float(atom[1]), float(atom[2]), float(atom[3])])
-
-    coords = np.asarray(positions).reshape(-1, 3)
-    return Structure(lattice, elements, coords, coords_are_cartesian=True)
+import re
+from typing import List, Union
+
+import numpy as np
+from pymatgen.core import Structure
+
+from dspawpy.io.read import get_lines_without_comment, get_sinfo
+
+
+def build_Structures_from_datafile(
+    datafile: Union[str, List[str]], si=None, ele=None, ai=None, fmt=None
+) -> List[Structure]:
+    r"""读取一/多个h5/json文件，返回pymatgen的Structures列表
+
+    Parameters
+    ----------
+    datafile : str or list
+        - h5/json/as/hzw/cif/poscar/cssr/xsf/mcsqs/prismatic/yaml/fleur-inpgen文件路径;
+        - 若给定字符串列表，将依次读取数据并合并成一个Structures列表
+    si: int, list or str
+        - 构型编号，从 1 开始
+
+            - si=1, 读取第一个构型
+            - si=[1,2], 读取第一个和第二个构型
+            - si=':', 读取所有构型
+            - si='-3:', 读取最后三个构型
+        - 若为空，多构型文件将读取所有构型，单构型文件将读取最新构型
+        - 此参数仅对 h5/json 文件有效
+    ele: str or list
+        - 元素符号，写法参考：'H' 或 ['H','O']
+        - 若为空，将读取所有元素的原子信息
+        - 此参数仅对 h5/json 文件有效
+    ai: int or list or str
+        - 原子编号，从 1 开始
+        - 用法同si
+        - 若为空，将读取所有原子信息
+        - 此参数仅对 h5/json 文件有效
+    fmt: str
+        - 文件格式，包括 'h5', 'json', 'as', 'hzw' 四种，其他值将被忽略。
+        - 若为空，文件类型将依据文件名称惯例判断。
+
+    Returns
+    -------
+    pymatgen_Structures : List[Structure]
+        结构列表
+
+    Examples
+    --------
+
+    >>> from dspawpy.io.structure import build_Structures_from_datafile as bs
+
+    读取单个文件生成 Structures 列表，支持四种类型
+
+    >>> pymatgen_Structures = bs(datafile='/data/home/hzw1002/dspawpy_repo/test/2.1/relax.h5')
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.1/relax.h5...
+    >>> len(pymatgen_Structures)
+    3
+    >>> pymatgen_Structures = bs(datafile='/data/home/hzw1002/dspawpy_repo/test/2.1/relax.json')
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.1/relax.json...
+     json所含数据默认仅保留到小数点后四位，与h5或log文件中所记载的数据存在一定误差，可能导致后续保存的结构文件不一致！可以考虑使用io.jsonPrec参数调整精度！
+    Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info...
+    >>> len(pymatgen_Structures)
+    3
+    >>> pymatgen_Structures = bs(datafile='/data/home/hzw1002/dspawpy_repo/test/supplement/PtH.as')
+    >>> len(pymatgen_Structures)
+    1
+    >>> pymatgen_Structures = bs(datafile='/data/home/hzw1002/dspawpy_repo/test/supplement/PtH.hzw')
+    build from hzw file may lack mag & fix info!
+    >>> len(pymatgen_Structures)
+    1
+
+    注意pymatgen_Structures是由多个 Structure 对象组成的列表，每个 Structure 对象分别对应一个构型。如果只有一个构型，也会返回列表，请使用 pymatgen_Structures[0] 获取 Structure 对象
+
+    当datafile为列表时，将依次读取多个文件，合并成一个Structures列表
+
+    >>> pymatgen_Structures = bs(datafile=['/data/home/hzw1002/dspawpy_repo/test/supplement/aimd1.h5','/data/home/hzw1002/dspawpy_repo/test/supplement/aimd2.h5'])
+    Reading /data/home/hzw1002/dspawpy_repo/test/supplement/aimd1.h5...
+    Reading /data/home/hzw1002/dspawpy_repo/test/supplement/aimd2.h5...
+    """
+    dfs = []
+    if isinstance(datafile, list):  # 续算模式，给的是多个文件
+        dfs = datafile
+    else:  # 单次计算模式，处理单个文件
+        dfs.append(datafile)
+
+    # 读取结构数据
+    pymatgen_Structures = []
+    for df in dfs:
+        structure_list = _get_structure_list(df, si, ele, ai, fmt)
+        pymatgen_Structures.extend(structure_list)
+
+    return pymatgen_Structures
+
+
+def _get_structure_list(
+    df: str, si=None, ele=None, ai=None, fmt=None
+) -> List[Structure]:
+    """get pymatgen structures from single datafile
+
+    Parameters
+    ----------
+    df : str
+        datafile
+
+    Returns
+    -------
+    List[Structure] : list of pymatgen structures
+    """
+
+    if fmt is None:
+        fmt = df.split(".")[-1]
+    else:
+        assert isinstance(fmt, str), "fmt must be str"
+
+    if fmt == "as":
+        strs = [_from_dspaw_as(df)]
+    elif fmt == "hzw":
+        print("build from hzw file may lack mag & fix info!")
+        strs = [_from_hzw(df)]
+    elif fmt == "h5" or fmt == "json":
+        Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
+            datafile=df, si=si, ele=ele, ai=ai
+        )  # returned positions, not scaled-positions
+        # remove _ from elements
+        elements = [re.sub(r"_", "", e) for e in elements]
+
+        strs = []
+        for i in range(Nstep):
+            if D_mag_fix:
+                strs.append(
+                    Structure(
+                        lattices[i],
+                        elements,
+                        positions[i],
+                        coords_are_cartesian=True,
+                        site_properties={k: v[i] for k, v in D_mag_fix.items()},
+                    )
+                )
+            else:
+                strs.append(
+                    Structure(
+                        lattices[i],
+                        elements,
+                        positions[i],
+                        coords_are_cartesian=True,
+                    )
+                )
+    else:
+        strs = [Structure.from_file(df)]
+
+    return strs
+
+
+def _from_dspaw_as(as_file: str = "structure.as") -> Structure:
+    """从DSPAW的as结构文件中读取结构信息
+
+    Parameters
+    ----------
+    as_file : str
+        DSPAW的as结构文件, 默认'structure.as'
+
+    Returns
+    -------
+    Structure
+        pymatgen的Structure对象
+    """
+
+    lines = get_lines_without_comment(as_file, "#")
+    N = int(lines[1])  # number of atoms
+
+    # parse lattice info
+    lattice = []  # lattice matrix
+    for line in lines[3:6]:
+        vector = line.split()
+        lattice.extend([float(vector[0]), float(vector[1]), float(vector[2])])
+    lattice = np.asarray(lattice).reshape(3, 3)
+
+    lat_fixs = []
+    if lines[2].strip() != "Lattice":  # fix lattice
+        lattice_fix_info = lines[2].strip().split()[1:]
+        if lattice_fix_info == ["Fix_x", "Fix_y", "Fix_z"]:
+            # ONLY support xyz fix in sequence, yzx will cause error
+            for line in lines[3:6]:
+                lfs = line.strip().split()[3:6]
+                for lf in lfs:
+                    if lf.startswith("T"):
+                        lat_fixs.append("True")
+                    elif lf.startswith("F"):
+                        lat_fixs.append("False")
+        elif lattice_fix_info == ["Fix"]:
+            for line in lines[3:6]:
+                lf = line.strip().split()[3]
+                if lf.startswith("T"):
+                    lat_fixs.append("True")
+                elif lf.startswith("F"):
+                    lat_fixs.append("False")
+        else:
+            raise ValueError("Lattice fix info error!")
+
+    elements = []
+    positions = []
+    for i in range(N):
+        atom = lines[i + 7].strip().split()
+        elements.append(atom[0])
+        positions.extend([float(atom[1]), float(atom[2]), float(atom[3])])
+
+    mf_info = None
+    l6 = lines[6].strip()  # str, 'Cartesian/Direct Mag Fix_x ...'
+    if l6 == "Direct":
+        is_direct = True
+    elif l6 == "Cartesian":
+        is_direct = False
+    else:
+        is_direct = l6.split()[0] == "Direct"
+        mf_info = l6.split()[1:]  # ['Mag', 'Fix_x', 'Fix_y', 'Fix_z']
+        for item in mf_info:
+            assert item in [
+                "Mag",
+                "Mag_x",
+                "Mag_y",
+                "Mag_z",
+                "Fix",
+                "Fix_x",
+                "Fix_y",
+                "Fix_z",
+            ], "Mag/Fix info error!"
+
+    mag_fix_dict = {}
+    if mf_info is not None:
+        for mf_index, item in enumerate(mf_info):
+            values = []
+            for i in range(N):
+                atom = lines[i + 7].strip().split()
+                mf = atom[4:]
+                values.append(mf[mf_index])
+
+            if item.startswith("Fix"):  # F -> False, T -> True
+                for value in values:
+                    if value.startswith("T"):
+                        values[values.index(value)] = "True"
+                    elif value.startswith("F"):
+                        values[values.index(value)] = "False"
+            mag_fix_dict[item] = values
+
+    if lat_fixs != []:
+        # replicate lat_fixs to N atoms
+        mag_fix_dict["LatticeFixs"] = [lat_fixs for i in range(N)]
+
+    coords = np.asarray(positions).reshape(-1, 3)
+    # remove _ from elements
+    elements = [re.sub(r"_", "", e) for e in elements]
+
+    if mag_fix_dict == {}:
+        return Structure(
+            lattice, elements, coords, coords_are_cartesian=(not is_direct)
+        )
+    else:
+        return Structure(
+            lattice,
+            elements,
+            coords,
+            coords_are_cartesian=(not is_direct),
+            site_properties=mag_fix_dict,
+        )
+
+
+def _from_hzw(hzw_file) -> Structure:
+    """从hzw结构文件中读取结构信息
+
+    Parameters
+    ----------
+    hzw_file : str
+        hzw结构文件，以 .hzw 结尾
+
+    Returns
+    -------
+    Structure
+        pymatgen的Structure对象
+    """
+    lines = get_lines_without_comment(hzw_file, "%")
+    number_of_probes = int(lines[0])
+    if number_of_probes != 0:
+        raise ValueError("dspaw only support 0 probes hzw file")
+    lattice = []
+    for line in lines[1:4]:
+        vector = line.split()
+        lattice.extend([float(vector[0]), float(vector[1]), float(vector[2])])
+
+    lattice = np.asarray(lattice).reshape(3, 3)
+    N = int(lines[4])
+    elements = []
+    positions = []
+    for i in range(N):
+        atom = lines[i + 5].strip().split()
+        elements.append(atom[0])
+        positions.extend([float(atom[1]), float(atom[2]), float(atom[3])])
+
+    coords = np.asarray(positions).reshape(-1, 3)
+    return Structure(lattice, elements, coords, coords_are_cartesian=True)
```

## dspawpy/io/utils.py

```diff
@@ -1,942 +1,942 @@
-# ! some functions are copied from ase
-# see https://wiki.fysik.dtu.dk/ase/index.html
-
-import os
-from typing import List
-
-import numpy as np
-import pandas as pd
-from pymatgen.electronic_structure.core import OrbitalType
-from pymatgen.electronic_structure.dos import CompleteDos
-from scipy import integrate
-
-from dspawpy.io.read import get_ele_from_h5
-
-Na = 6.02214179e23  # 阿伏伽德罗常数 单位 /mol
-h = 6.6260696e-34  # 普朗克常数 单位J*s
-kB = 1.3806503e-23  # 玻尔兹曼常数 J/K
-R = Na * kB  # 理想气体常数 J/(K*mol)
-amu = 1.66053906660e-27  # 原子质量单位 kg
-k = 1.380649e-23 / 1.602176634e-19  # eV/K
-atomic_masses_iupac2016 = np.array(
-    [
-        1.0,  # X
-        1.008,  # H [1.00784, 1.00811]
-        4.002602,  # He
-        6.94,  # Li [6.938, 6.997]
-        9.0121831,  # Be
-        10.81,  # B [10.806, 10.821]
-        12.011,  # C [12.0096, 12.0116]
-        14.007,  # N [14.00643, 14.00728]
-        15.999,  # O [15.99903, 15.99977]
-        18.998403163,  # F
-        20.1797,  # Ne
-        22.98976928,  # Na
-        24.305,  # Mg [24.304, 24.307]
-        26.9815385,  # Al
-        28.085,  # Si [28.084, 28.086]
-        30.973761998,  # P
-        32.06,  # S [32.059, 32.076]
-        35.45,  # Cl [35.446, 35.457]
-        39.948,  # Ar
-        39.0983,  # K
-        40.078,  # Ca
-        44.955908,  # Sc
-        47.867,  # Ti
-        50.9415,  # V
-        51.9961,  # Cr
-        54.938044,  # Mn
-        55.845,  # Fe
-        58.933194,  # Co
-        58.6934,  # Ni
-        63.546,  # Cu
-        65.38,  # Zn
-        69.723,  # Ga
-        72.630,  # Ge
-        74.921595,  # As
-        78.971,  # Se
-        79.904,  # Br [79.901, 79.907]
-        83.798,  # Kr
-        85.4678,  # Rb
-        87.62,  # Sr
-        88.90584,  # Y
-        91.224,  # Zr
-        92.90637,  # Nb
-        95.95,  # Mo
-        97.90721,  # 98Tc
-        101.07,  # Ru
-        102.90550,  # Rh
-        106.42,  # Pd
-        107.8682,  # Ag
-        112.414,  # Cd
-        114.818,  # In
-        118.710,  # Sn
-        121.760,  # Sb
-        127.60,  # Te
-        126.90447,  # I
-        131.293,  # Xe
-        132.90545196,  # Cs
-        137.327,  # Ba
-        138.90547,  # La
-        140.116,  # Ce
-        140.90766,  # Pr
-        144.242,  # Nd
-        144.91276,  # 145Pm
-        150.36,  # Sm
-        151.964,  # Eu
-        157.25,  # Gd
-        158.92535,  # Tb
-        162.500,  # Dy
-        164.93033,  # Ho
-        167.259,  # Er
-        168.93422,  # Tm
-        173.054,  # Yb
-        174.9668,  # Lu
-        178.49,  # Hf
-        180.94788,  # Ta
-        183.84,  # W
-        186.207,  # Re
-        190.23,  # Os
-        192.217,  # Ir
-        195.084,  # Pt
-        196.966569,  # Au
-        200.592,  # Hg
-        204.38,  # Tl [204.382, 204.385]
-        207.2,  # Pb
-        208.98040,  # Bi
-        208.98243,  # 209Po
-        209.98715,  # 210At
-        222.01758,  # 222Rn
-        223.01974,  # 223Fr
-        226.02541,  # 226Ra
-        227.02775,  # 227Ac
-        232.0377,  # Th
-        231.03588,  # Pa
-        238.02891,  # U
-        237.04817,  # 237Np
-        244.06421,  # 244Pu
-        243.06138,  # 243Am
-        247.07035,  # 247Cm
-        247.07031,  # 247Bk
-        251.07959,  # 251Cf
-        252.0830,  # 252Es
-        257.09511,  # 257Fm
-        258.09843,  # 258Md
-        259.1010,  # 259No
-        262.110,  # 262Lr
-        267.122,  # 267Rf
-        268.126,  # 268Db
-        271.134,  # 271Sg
-        270.133,  # 270Bh
-        269.1338,  # 269Hs
-        278.156,  # 278Mt
-        281.165,  # 281Ds
-        281.166,  # 281Rg
-        285.177,  # 285Cn
-        286.182,  # 286Nh
-        289.190,  # 289Fl
-        289.194,  # 289Mc
-        293.204,  # 293Lv
-        293.208,  # 293Ts
-        294.214,  # 294Og
-    ]
-)
-
-chemical_symbols = [
-    # 0
-    "X",
-    # 1
-    "H",
-    "He",
-    # 2
-    "Li",
-    "Be",
-    "B",
-    "C",
-    "N",
-    "O",
-    "F",
-    "Ne",
-    # 3
-    "Na",
-    "Mg",
-    "Al",
-    "Si",
-    "P",
-    "S",
-    "Cl",
-    "Ar",
-    # 4
-    "K",
-    "Ca",
-    "Sc",
-    "Ti",
-    "V",
-    "Cr",
-    "Mn",
-    "Fe",
-    "Co",
-    "Ni",
-    "Cu",
-    "Zn",
-    "Ga",
-    "Ge",
-    "As",
-    "Se",
-    "Br",
-    "Kr",
-    # 5
-    "Rb",
-    "Sr",
-    "Y",
-    "Zr",
-    "Nb",
-    "Mo",
-    "Tc",
-    "Ru",
-    "Rh",
-    "Pd",
-    "Ag",
-    "Cd",
-    "In",
-    "Sn",
-    "Sb",
-    "Te",
-    "I",
-    "Xe",
-    # 6
-    "Cs",
-    "Ba",
-    "La",
-    "Ce",
-    "Pr",
-    "Nd",
-    "Pm",
-    "Sm",
-    "Eu",
-    "Gd",
-    "Tb",
-    "Dy",
-    "Ho",
-    "Er",
-    "Tm",
-    "Yb",
-    "Lu",
-    "Hf",
-    "Ta",
-    "W",
-    "Re",
-    "Os",
-    "Ir",
-    "Pt",
-    "Au",
-    "Hg",
-    "Tl",
-    "Pb",
-    "Bi",
-    "Po",
-    "At",
-    "Rn",
-    # 7
-    "Fr",
-    "Ra",
-    "Ac",
-    "Th",
-    "Pa",
-    "U",
-    "Np",
-    "Pu",
-    "Am",
-    "Cm",
-    "Bk",
-    "Cf",
-    "Es",
-    "Fm",
-    "Md",
-    "No",
-    "Lr",
-    "Rf",
-    "Db",
-    "Sg",
-    "Bh",
-    "Hs",
-    "Mt",
-    "Ds",
-    "Rg",
-    "Cn",
-    "Nh",
-    "Fl",
-    "Mc",
-    "Lv",
-    "Ts",
-    "Og",
-]
-
-atomic_numbers = {}
-for Z, symbol in enumerate(chemical_symbols):
-    atomic_numbers[symbol] = Z
-
-
-def eles2masses(eles: List[str]) -> List[float]:
-    """将元素列表转换为质量列表
-
-    Parameters
-    ----------
-    eles : List[str]
-        元素列表
-
-    Returns
-    -------
-    List[float]
-        质量列表
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import eles2masses
-    >>> eles = ["H", "O"]
-    >>> masses = eles2masses(eles)
-    >>> masses
-    array([ 1.008, 15.999])
-    """
-    masses = []
-    for e in eles:
-        masses.append(atomic_masses_iupac2016[atomic_numbers[e]])
-    return np.array(masses)
-
-
-def get_ma(elements, positions, Natom):
-    """Get the moments of inertia along the principal axes.
-
-    The three principal moments of inertia are computed from the
-    eigenvalues of the symmetric inertial tensor. Periodic boundary
-    conditions are ignored. Units of the moments of inertia are
-    amu*angstrom**2.
-    """
-    masses = eles2masses(elements)
-    com = np.dot(masses, positions) / masses.sum()
-    positions -= com  # translate center of mass to origin
-    masses = eles2masses(elements)
-
-    # Initialize elements of the inertial tensor
-    I11 = I22 = I33 = I12 = I13 = I23 = 0.0
-    for i in range(Natom):
-        x, y, z = positions[i]
-        m = masses[i]
-
-        I11 += m * (y**2 + z**2)
-        I22 += m * (x**2 + z**2)
-        I33 += m * (x**2 + y**2)
-        I12 += -m * x * y
-        I13 += -m * x * z
-        I23 += -m * y * z
-
-    I = np.array([[I11, I12, I13], [I12, I22, I23], [I13, I23, I33]])
-
-    evals, evecs = np.linalg.eigh(I)
-    return evals
-
-
-class IdealGasThermo:
-    """import from ase.thermochemistry.IdealGasThermo
-
-    Parameters
-    ----------
-    vib_energies : list
-        List of vibrational energies in eV.
-    geometry : str
-        One of 'linear', 'nonlinear', 'monatomic'
-    potentialenergy : float
-        Potential energy in eV.
-    elements : list
-        such as ['H', 'O'].
-    symmetrynumber : int
-        Symmetry number.
-    spin : int
-        Spin multiplicity.
-    natoms : int
-        Number of atoms.
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import IdealGasThermo
-    >>> thermo = IdealGasThermo(vib_energies=[0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
-    ...                         geometry='linear', potentialenergy=0.,  # eV
-    ...                         elements=['H', 'O'], positions=[[0, 0, 0], [0, 0, 1]],  # angstrom
-    ...                         symmetrynumber=None, spin=None, natoms=None)
-    >>> thermo.get_enthalpy(298.15)  # K
-    Enthalpy components at T = 298.15 K:
-    ===============================
-    E_pot                  0.000 eV
-    E_ZPE                  0.300 eV
-    Cv_trans (0->T)        0.039 eV
-    Cv_rot (0->T)          0.026 eV
-    Cv_vib (0->T)          0.000 eV
-    (C_v -> C_p)           0.026 eV
-    -------------------------------
-    H                      0.390 eV
-    ===============================
-    0.389924026967057
-    """
-
-    # 读取elements数组代替atoms
-    def __init__(
-        self,
-        vib_energies,
-        geometry,
-        potentialenergy=0.0,
-        elements=None,
-        positions=None,
-        symmetrynumber=None,
-        spin=None,
-        natoms=None,
-    ):
-        self.potentialenergy = potentialenergy
-        self.geometry = geometry
-        self.elements = elements
-        if isinstance(positions, list):
-            self.positions = np.array(positions, dtype=float)
-        elif isinstance(positions, np.ndarray):
-            self.positions = positions
-        else:
-            raise TypeError("positions must be list or np.ndarray")
-        if isinstance(vib_energies, list):
-            vib_energies = np.array(vib_energies)
-        elif isinstance(vib_energies, np.ndarray):
-            pass
-        else:
-            raise TypeError("vib_energies must be list or np.ndarray")
-        self.sigma = symmetrynumber
-        self.spin = spin
-        if natoms is None:
-            if elements:
-                natoms = len(elements)
-        # Cut the vibrations to those needed from the geometry.
-        if natoms:
-            if geometry == "nonlinear":
-                self.vib_energies = vib_energies[-(3 * natoms - 6) :]
-            elif geometry == "linear":
-                self.vib_energies = vib_energies[-(3 * natoms - 5) :]
-            elif geometry == "monatomic":
-                self.vib_energies = []
-        else:
-            self.vib_energies = vib_energies
-        # Make sure no imaginary frequencies remain.
-        if sum(np.iscomplex(self.vib_energies)):
-            raise ValueError("Imaginary frequencies are present.")
-        else:
-            self.vib_energies = np.real(self.vib_energies)  # clear +0.j
-        self.referencepressure = 1.0e5  # Pa
-        self.natoms = natoms
-
-    def get_ZPE_correction(self):
-        """Returns the zero-point vibrational energy correction in eV."""
-        zpe = 0.0
-        for energy in self.vib_energies:
-            zpe += 0.5 * energy
-        return zpe
-
-    def _vibrational_energy_contribution(self, temperature):
-        """Calculates the change in internal energy due to vibrations from
-        0K to the specified temperature for a set of vibrations given in
-        eV and a temperature given in Kelvin. Returns the energy change
-        in eV."""
-        kT = k * temperature
-        dU = 0.0
-        for energy in self.vib_energies:
-            dU += energy / (np.exp(energy / kT) - 1.0)
-        return dU
-
-    def _vibrational_entropy_contribution(self, temperature):
-        """Calculates the entropy due to vibrations for a set of vibrations
-        given in eV and a temperature given in Kelvin.  Returns the entropy
-        in eV/K."""
-        kT = k * temperature
-        S_v = 0.0
-        for energy in self.vib_energies:
-            x = energy / kT
-            S_v += x / (np.exp(x) - 1.0) - np.log(1.0 - np.exp(-x))
-        S_v *= k
-        return S_v
-
-    def get_enthalpy(self, temperature):
-        """Returns the enthalpy, in eV, in the ideal gas approximation
-        at a specified temperature (K)."""
-
-        fmt = "%-15s%13.3f eV"
-        print("Enthalpy components at T = %.2f K:" % temperature)
-        print("=" * 31)
-
-        H = 0.0
-
-        print(fmt % ("E_pot", self.potentialenergy))
-        H += self.potentialenergy
-
-        zpe = self.get_ZPE_correction()
-        print(fmt % ("E_ZPE", zpe))
-        H += zpe
-
-        Cv_t = 3.0 / 2.0 * k  # translational heat capacity (3-d gas)
-        print(fmt % ("Cv_trans (0->T)", Cv_t * temperature))
-        H += Cv_t * temperature
-
-        if self.geometry == "nonlinear":  # rotational heat capacity
-            Cv_r = 3.0 / 2.0 * k
-        elif self.geometry == "linear":
-            Cv_r = k
-        elif self.geometry == "monatomic":
-            Cv_r = 0.0
-        print(fmt % ("Cv_rot (0->T)", Cv_r * temperature))
-        H += Cv_r * temperature
-
-        dH_v = self._vibrational_energy_contribution(temperature)
-        print(fmt % ("Cv_vib (0->T)", dH_v))
-        H += dH_v
-
-        Cp_corr = k * temperature
-        print(fmt % ("(C_v -> C_p)", Cp_corr))
-        H += Cp_corr
-
-        print("-" * 31)
-        print(fmt % ("H", H))
-        print("=" * 31)
-        return H
-
-    def get_entropy(self, temperature, pressure):
-        """Returns the entropy, in eV/K, in the ideal gas approximation
-        at a specified temperature (K) and pressure (Pa)."""
-
-        if self.elements is None or self.sigma is None or self.spin is None:
-            raise RuntimeError(
-                "elements, symmetrynumber, and spin must be "
-                "specified for entropy and free energy "
-                "calculations."
-            )
-        S = 0.0
-        # Translational entropy (term inside the log is in SI units).
-        mass = sum(eles2masses(self.elements)) * amu  # kg/molecule
-        S_t = (2 * np.pi * mass * kB * temperature / h**2) ** (3.0 / 2)
-        S_t *= kB * temperature / self.referencepressure
-        S_t = k * (np.log(S_t) + 5.0 / 2.0)
-        S += S_t
-
-        # Rotational entropy (term inside the log is in SI units).
-        if self.geometry == "monatomic":
-            S_r = 0.0
-        elif self.geometry == "nonlinear":
-            inertias = (
-                get_ma(self.elements, self.positions, self.natoms)
-                * amu
-                / (10.0**10) ** 2
-            )  # kg m^2
-            S_r = np.sqrt(np.pi * np.product(inertias)) / self.sigma
-            S_r *= (8.0 * np.pi**2 * kB * temperature / h**2) ** (3.0 / 2.0)
-            S_r = k * (np.log(S_r) + 3.0 / 2.0)
-        elif self.geometry == "linear":
-            inertias = (
-                get_ma(self.elements, self.positions, self.natoms)
-                * amu
-                / (10.0**10) ** 2
-            )  # kg m^2
-            inertia = max(inertias)  # should be two identical and one zero
-            S_r = 8 * np.pi**2 * inertia * kB * temperature / self.sigma / h**2
-            S_r = k * (np.log(S_r) + 1.0)
-        S += S_r
-        # Electronic entropy.
-        S_e = k * np.log(2 * self.spin + 1)
-        S += S_e
-        # Vibrational entropy.
-        S_v = self._vibrational_entropy_contribution(temperature)
-        S += S_v
-        # Pressure correction to translational entropy.
-        S_p = -k * np.log(pressure / self.referencepressure)
-        S += S_p
-        return S
-
-    def get_gibbs_energy(self, temperature, pressure):
-        """Returns the Gibbs free energy, in eV, in the ideal gas
-        approximation at a specified temperature (K) and pressure (Pa)."""
-
-        H = self.get_enthalpy(temperature)
-        print("")
-        S = self.get_entropy(temperature, pressure)
-        G = H - temperature * S
-
-        print("")
-        print(
-            "Free energy components at T = %.2f K and P = %.1f Pa:"
-            % (temperature, pressure)
-        )
-        print("=" * 23)
-        fmt = "%5s%15.3f eV"
-        print(fmt % ("H", H))
-        print(fmt % ("-T*S", -temperature * S))
-        print("-" * 23)
-        print(fmt % ("G", G))
-        print("=" * 23)
-        return G
-
-
-def getTSgas(
-    fretxt="frequency.txt",
-    datafile=".",
-    potentialenergy=0,  # eV
-    elements=None,
-    geometry="linear",
-    positions=None,  # Angstrom
-    symmetrynumber=1,
-    spin=1,
-    temperature=298.15,
-    pressure=101325,
-):
-    """理想气体近似下，计算熵的能量贡献
-
-
-    Parameters
-    ----------
-    fretxt : str
-        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
-    datafile : str
-        计算结果json或h5文件或包含它们的文件夹路径, 默认当前路径；
-        如果设置为None，则需要传入elements和positions参数
-    potentialenergy : float
-        势能，单位eV
-    elements : list
-        元素列表，如果
-    geometry : str
-        分子几何，monatomic, linear, nonlinear
-    positions : list
-        原子坐标，单位Angstrom
-    symmetrynumber : int
-        对称数
-    spin : int
-        自旋数
-    temperature : float
-        温度，单位K
-    pressure : float
-        压强，单位Pa
-
-    Returns
-    -------
-    TSgas : float
-        理想气体近似下，计算熵的能量贡献，单位eV
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import getTSgas
-    >>> TSgas = getTSgas(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', datafile='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.h5', potentialenergy=-0.0,  geometry='linear', symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
-    >>> print(TSgas)
-    0.8515317035550232
-    >>> TSgas = getTSgas(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', datafile='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.h5', potentialenergy=-0.0,  geometry='linear', symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
-    >>> TSgas
-    0.8515317035550232
-    """
-    ve = []
-    with open(fretxt) as ft:
-        lines = ft.readlines()
-        for i in range(2, len(lines)):
-            if lines[i].strip()[1] == "f/i":
-                ve.append(complex(lines[i].split()[-1]) / 1000)
-            else:
-                ve.append(float(lines[i].split()[-1]) / 1000)
-
-    if datafile:  # skip if datafile is None
-        # search datafile in the given directory
-        if os.path.isdir(datafile):
-            directory = datafile  # specified datafile is actually a directory
-            print("您指定了一个文件夹，正在查找相关h5或json文件...")
-            if os.path.exists(os.path.join(directory, "frequency.h5")):
-                datafile = os.path.join(directory, "frequency.h5")
-                print("Reading frequency.h5...")
-            elif os.path.exists(os.path.join(directory, "frequency.json")):
-                datafile = os.path.join(directory, "frequency.json")
-                print("Reading frequency.json...")
-            else:
-                raise FileNotFoundError("未找到frequency.h5/frequency.json文件！")
-        if datafile.endswith(".h5"):
-            eles = get_ele_from_h5(datafile)
-            import h5py
-
-            data = h5py.File(datafile)
-            poses = np.array(data.get("/AtomInfo/Position")).reshape(-1, 3)
-
-        elif datafile.endswith(".json"):
-            import json
-
-            with open(datafile) as f:
-                data = json.load(f)
-            atoms = data["AtomInfo"]["Atoms"]
-            eles = []
-            poses = []
-            for i in range(len(atoms)):
-                eles.append(atoms[i]["Element"])
-                poses.append(atoms[i]["Position"])
-        else:
-            raise TypeError("仅支持读取h5或json文件！")
-    else:
-        eles = elements
-        poses = positions
-
-    # 计算熵的能量贡献
-    thermo = IdealGasThermo(
-        vib_energies=ve,  # eV
-        potentialenergy=potentialenergy,  # eV
-        elements=eles,
-        geometry=geometry,
-        positions=poses,  # Angstrom
-        symmetrynumber=symmetrynumber,
-        spin=spin,
-    )
-    S = thermo.get_entropy(temperature, pressure)
-
-    return S * temperature
-
-
-def d_band(spin, dos_data: CompleteDos):  # 定义函数，括号里给出函数的两个变量
-    """计算d带中心
-
-    Parameters
-    ----------
-    spin : Spin.up或Spin.down
-        自旋类型，
-    dos_data : pymatgen.electronic_structure.dos.CompleteDos
-        dos数据
-
-    Returns
-    -------
-    db1 : float
-        d带中心数值
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import d_band
-    >>> from dspawpy.io.read import get_dos_data
-    >>> dos_data = get_dos_data("/data/home/hzw1002/dspawpy_repo/test/supplement/dos.h5")  # 从dos.h5中读取数据
-    >>> for spin in dos_data.densities:
-    ...     print(f'{spin=}')
-    ...     c = d_band(spin, dos_data)
-    ...     print(c)
-    spin=<Spin.up: 1>
-    -3.666508748164936
-    """
-    dos_d = dos_data.get_spd_dos()[OrbitalType.d]
-    # dos_d = dos_data.get_spd_dos()[d]
-    Efermi = dos_data.efermi
-    epsilon = dos_d.energies - Efermi  # shift d-band center
-
-    N1 = dos_d.densities[spin]
-    M1 = epsilon * N1
-    SummaM1 = integrate.simps(M1, epsilon)
-    SummaN1 = integrate.simps(N1, epsilon)
-
-    return SummaM1 / SummaN1
-
-
-def getZPE(fretxt: str = "frequency.txt"):
-    """从fretext中读取数据，计算ZPE
-
-    将另外保存结果到 ZPE_TS.dat 中
-
-    Parameters
-    ----------
-    fretxt : str
-        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
-
-    Returns
-    -------
-    ZPE: float
-        零点能
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import getZPE
-    >>> ZPE= getZPE(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt')
-    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
-       Frequency (meV)
-    0       284.840033
-    <BLANKLINE>
-    正在写入ZPE.dat文件...
-    <BLANKLINE>
-    --> Zero-point energy,  ZPE (eV): 0.1424200165
-    >>> ZPE
-    0.1424200165
-    """
-
-    # 1. read data
-    data_get_ZPE = []
-    with open(fretxt, "r") as f:
-        for line in f.readlines():
-            data_line = line.strip().split()
-            if len(data_line) != 6:
-                continue
-            if data_line[1] == "f":
-                data_get_ZPE.append(float(data_line[5]))
-
-    data_get_ZPE = np.array(data_get_ZPE)
-
-    # 2. printout to check
-    print(f"=== 从{fretxt}中读取到的相关如下 ===")
-    dt = pd.DataFrame({"Frequency (meV)": data_get_ZPE}, index=None)
-    print(dt)
-
-    if len(data_get_ZPE) == 0:
-        raise ValueError("全是虚频，请考虑重新优化结构...")
-    else:
-        print("\n正在写入ZPE.dat文件...")
-        np.savetxt(
-            "ZPE.dat",
-            np.array(data_get_ZPE).T,
-            fmt="%.6f",
-            header="Frequency (meV)",
-            comments=f"Data read from {os.path.abspath(fretxt)}\n",
-        )
-
-    # 3. calculate
-    ZPE = 0
-    for data in data_get_ZPE:
-        ZPE += data / 2000.0
-    print("\n--> Zero-point energy,  ZPE (eV):", ZPE)
-
-    with open("ZPE.dat", "a") as f:
-        f.write(f"\n--> Zero-point energy,  ZPE (eV): {ZPE}")
-
-    return ZPE
-
-
-def getTSads(fretxt: str = "frequency.txt", T: float = 298.15):
-    """从fretext中读取数据，计算ZPE和TS
-
-    将另外保存结果到 ZPE_TS.dat 中
-
-    Parameters
-    ----------
-    fretxt : str
-        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
-    T : float
-        温度，单位K, 默认298.15
-
-    Returns
-    -------
-    TS: float
-        熵校正
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import getTSads
-    >>> TS = getTSads(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', T=298.15)
-    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
-       Frequency (THz)
-    0        68.873993
-    <BLANKLINE>
-    正在写入TS.dat文件...
-    --> Entropy contribution, T*S (eV)： 4.7566997225177686e-06
-    >>> TS
-    4.7566997225177686e-06
-    """
-    data_get_TS = []
-    with open(fretxt, "r") as f:
-        for line in f.readlines():
-            data_line = line.strip().split()
-            if len(data_line) != 6:
-                continue
-            if data_line[1] == "f":
-                data_get_TS.append(float(data_line[2]))
-
-    data_get_TS = np.array(data_get_TS)
-
-    # 2. printout to check
-    print(f"=== 从{fretxt}中读取到的相关如下 ===")
-    dt = pd.DataFrame({"Frequency (THz)": data_get_TS}, index=None)
-    print(dt)
-
-    if len(data_get_TS) == 0:
-        raise ValueError("全是虚频，请考虑重新优化结构...")
-    else:
-        print("\n正在写入TS.dat文件...")
-        np.savetxt(
-            "TS.dat",
-            np.array(data_get_TS).T,
-            fmt="%.6f",
-            header="Frequency (THz)",
-            comments=f"Data read from {os.path.abspath(fretxt)}\n",
-        )
-
-    # 3. calculate
-    sum_S = 0
-    import math  # 因为要使用 e的多少次方，ln（）对数
-
-    for vi_THz in data_get_TS:
-        vi_Hz = vi_THz * 1e12
-        m1 = h * Na * vi_Hz
-        m2 = h * vi_Hz / (kB * T)
-        m3 = math.exp(m2) - 1
-        m4 = T * m3
-        m5 = 1 - math.exp(-m2)  # math.exp(3) 就是e的3次方
-        m6 = math.log(m5, math.e)  # m6= ln(m5)   math.e在python中=e ，以右边为底的对数
-        m7 = R * m6
-        m8 = m1 / m4 - m7  # S 单位J/(mol*K)
-        m9 = (T * m8 / 1000) / 96.49  # T*S,将单位化为KJ/mol, 96.49 kJ/mol = 1 eV 单位eV
-        sum_S += m9
-
-    print("--> Entropy contribution, T*S (eV)：", sum_S)
-
-    with open("ZPE_TS.dat", "a") as f:
-        f.write(f"\n--> Entropy contribution, T*S (eV): {sum_S}\n")
-
-    return sum_S
-
-
-def thermo_correction(fretxt: str = "frequency.txt", T: float = 298.15):
-    """从fretext中读取数据，计算ZPE和TS
-    将另外保存结果到 ZPE_TS.dat 中
-
-    Parameters
-    ----------
-    fretxt : str
-        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
-    T : float
-        温度，单位K, 默认298.15
-
-    Returns
-    -------
-    ZPE: float
-        零点能
-    TS: float
-        熵校正
-
-    Examples
-    --------
-    >>> from dspawpy.io.utils import thermo_correction
-    >>> ZPE, TS = thermo_correction(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', T=298.15)
-    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
-       Frequency (meV)
-    0       284.840033
-    <BLANKLINE>
-    正在写入ZPE.dat文件...
-    <BLANKLINE>
-    --> Zero-point energy,  ZPE (eV): 0.1424200165
-    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
-       Frequency (THz)
-    0        68.873993
-    <BLANKLINE>
-    正在写入TS.dat文件...
-    --> Entropy contribution, T*S (eV)： 4.7566997225177686e-06
-    >>> ZPE
-    0.1424200165
-    >>> TS
-    4.7566997225177686e-06
-    """
-
-    ZPE = getZPE(fretxt=fretxt)
-    sum_S = getTSads(fretxt=fretxt, T=T)
-
-    return ZPE, sum_S
-
-
-def _symbols2numbers(symbols) -> List[int]:
-    numbers = []
-    for s in symbols:
-        if isinstance(s, str):
-            numbers.append(atomic_numbers[s])
-        else:
-            numbers.append(int(s))
-    return numbers
+# ! some functions are copied from ase
+# see https://wiki.fysik.dtu.dk/ase/index.html
+
+import os
+from typing import List
+
+import numpy as np
+import pandas as pd
+from pymatgen.electronic_structure.core import OrbitalType
+from pymatgen.electronic_structure.dos import CompleteDos
+from scipy import integrate
+
+from dspawpy.io.read import get_ele_from_h5
+
+Na = 6.02214179e23  # 阿伏伽德罗常数 单位 /mol
+h = 6.6260696e-34  # 普朗克常数 单位J*s
+kB = 1.3806503e-23  # 玻尔兹曼常数 J/K
+R = Na * kB  # 理想气体常数 J/(K*mol)
+amu = 1.66053906660e-27  # 原子质量单位 kg
+k = 1.380649e-23 / 1.602176634e-19  # eV/K
+atomic_masses_iupac2016 = np.array(
+    [
+        1.0,  # X
+        1.008,  # H [1.00784, 1.00811]
+        4.002602,  # He
+        6.94,  # Li [6.938, 6.997]
+        9.0121831,  # Be
+        10.81,  # B [10.806, 10.821]
+        12.011,  # C [12.0096, 12.0116]
+        14.007,  # N [14.00643, 14.00728]
+        15.999,  # O [15.99903, 15.99977]
+        18.998403163,  # F
+        20.1797,  # Ne
+        22.98976928,  # Na
+        24.305,  # Mg [24.304, 24.307]
+        26.9815385,  # Al
+        28.085,  # Si [28.084, 28.086]
+        30.973761998,  # P
+        32.06,  # S [32.059, 32.076]
+        35.45,  # Cl [35.446, 35.457]
+        39.948,  # Ar
+        39.0983,  # K
+        40.078,  # Ca
+        44.955908,  # Sc
+        47.867,  # Ti
+        50.9415,  # V
+        51.9961,  # Cr
+        54.938044,  # Mn
+        55.845,  # Fe
+        58.933194,  # Co
+        58.6934,  # Ni
+        63.546,  # Cu
+        65.38,  # Zn
+        69.723,  # Ga
+        72.630,  # Ge
+        74.921595,  # As
+        78.971,  # Se
+        79.904,  # Br [79.901, 79.907]
+        83.798,  # Kr
+        85.4678,  # Rb
+        87.62,  # Sr
+        88.90584,  # Y
+        91.224,  # Zr
+        92.90637,  # Nb
+        95.95,  # Mo
+        97.90721,  # 98Tc
+        101.07,  # Ru
+        102.90550,  # Rh
+        106.42,  # Pd
+        107.8682,  # Ag
+        112.414,  # Cd
+        114.818,  # In
+        118.710,  # Sn
+        121.760,  # Sb
+        127.60,  # Te
+        126.90447,  # I
+        131.293,  # Xe
+        132.90545196,  # Cs
+        137.327,  # Ba
+        138.90547,  # La
+        140.116,  # Ce
+        140.90766,  # Pr
+        144.242,  # Nd
+        144.91276,  # 145Pm
+        150.36,  # Sm
+        151.964,  # Eu
+        157.25,  # Gd
+        158.92535,  # Tb
+        162.500,  # Dy
+        164.93033,  # Ho
+        167.259,  # Er
+        168.93422,  # Tm
+        173.054,  # Yb
+        174.9668,  # Lu
+        178.49,  # Hf
+        180.94788,  # Ta
+        183.84,  # W
+        186.207,  # Re
+        190.23,  # Os
+        192.217,  # Ir
+        195.084,  # Pt
+        196.966569,  # Au
+        200.592,  # Hg
+        204.38,  # Tl [204.382, 204.385]
+        207.2,  # Pb
+        208.98040,  # Bi
+        208.98243,  # 209Po
+        209.98715,  # 210At
+        222.01758,  # 222Rn
+        223.01974,  # 223Fr
+        226.02541,  # 226Ra
+        227.02775,  # 227Ac
+        232.0377,  # Th
+        231.03588,  # Pa
+        238.02891,  # U
+        237.04817,  # 237Np
+        244.06421,  # 244Pu
+        243.06138,  # 243Am
+        247.07035,  # 247Cm
+        247.07031,  # 247Bk
+        251.07959,  # 251Cf
+        252.0830,  # 252Es
+        257.09511,  # 257Fm
+        258.09843,  # 258Md
+        259.1010,  # 259No
+        262.110,  # 262Lr
+        267.122,  # 267Rf
+        268.126,  # 268Db
+        271.134,  # 271Sg
+        270.133,  # 270Bh
+        269.1338,  # 269Hs
+        278.156,  # 278Mt
+        281.165,  # 281Ds
+        281.166,  # 281Rg
+        285.177,  # 285Cn
+        286.182,  # 286Nh
+        289.190,  # 289Fl
+        289.194,  # 289Mc
+        293.204,  # 293Lv
+        293.208,  # 293Ts
+        294.214,  # 294Og
+    ]
+)
+
+chemical_symbols = [
+    # 0
+    "X",
+    # 1
+    "H",
+    "He",
+    # 2
+    "Li",
+    "Be",
+    "B",
+    "C",
+    "N",
+    "O",
+    "F",
+    "Ne",
+    # 3
+    "Na",
+    "Mg",
+    "Al",
+    "Si",
+    "P",
+    "S",
+    "Cl",
+    "Ar",
+    # 4
+    "K",
+    "Ca",
+    "Sc",
+    "Ti",
+    "V",
+    "Cr",
+    "Mn",
+    "Fe",
+    "Co",
+    "Ni",
+    "Cu",
+    "Zn",
+    "Ga",
+    "Ge",
+    "As",
+    "Se",
+    "Br",
+    "Kr",
+    # 5
+    "Rb",
+    "Sr",
+    "Y",
+    "Zr",
+    "Nb",
+    "Mo",
+    "Tc",
+    "Ru",
+    "Rh",
+    "Pd",
+    "Ag",
+    "Cd",
+    "In",
+    "Sn",
+    "Sb",
+    "Te",
+    "I",
+    "Xe",
+    # 6
+    "Cs",
+    "Ba",
+    "La",
+    "Ce",
+    "Pr",
+    "Nd",
+    "Pm",
+    "Sm",
+    "Eu",
+    "Gd",
+    "Tb",
+    "Dy",
+    "Ho",
+    "Er",
+    "Tm",
+    "Yb",
+    "Lu",
+    "Hf",
+    "Ta",
+    "W",
+    "Re",
+    "Os",
+    "Ir",
+    "Pt",
+    "Au",
+    "Hg",
+    "Tl",
+    "Pb",
+    "Bi",
+    "Po",
+    "At",
+    "Rn",
+    # 7
+    "Fr",
+    "Ra",
+    "Ac",
+    "Th",
+    "Pa",
+    "U",
+    "Np",
+    "Pu",
+    "Am",
+    "Cm",
+    "Bk",
+    "Cf",
+    "Es",
+    "Fm",
+    "Md",
+    "No",
+    "Lr",
+    "Rf",
+    "Db",
+    "Sg",
+    "Bh",
+    "Hs",
+    "Mt",
+    "Ds",
+    "Rg",
+    "Cn",
+    "Nh",
+    "Fl",
+    "Mc",
+    "Lv",
+    "Ts",
+    "Og",
+]
+
+atomic_numbers = {}
+for Z, symbol in enumerate(chemical_symbols):
+    atomic_numbers[symbol] = Z
+
+
+def eles2masses(eles: List[str]) -> List[float]:
+    """将元素列表转换为质量列表
+
+    Parameters
+    ----------
+    eles : List[str]
+        元素列表
+
+    Returns
+    -------
+    List[float]
+        质量列表
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import eles2masses
+    >>> eles = ["H", "O"]
+    >>> masses = eles2masses(eles)
+    >>> masses
+    array([ 1.008, 15.999])
+    """
+    masses = []
+    for e in eles:
+        masses.append(atomic_masses_iupac2016[atomic_numbers[e]])
+    return np.array(masses)
+
+
+def get_ma(elements, positions, Natom):
+    """Get the moments of inertia along the principal axes.
+
+    The three principal moments of inertia are computed from the
+    eigenvalues of the symmetric inertial tensor. Periodic boundary
+    conditions are ignored. Units of the moments of inertia are
+    amu*angstrom**2.
+    """
+    masses = eles2masses(elements)
+    com = np.dot(masses, positions) / masses.sum()
+    positions -= com  # translate center of mass to origin
+    masses = eles2masses(elements)
+
+    # Initialize elements of the inertial tensor
+    I11 = I22 = I33 = I12 = I13 = I23 = 0.0
+    for i in range(Natom):
+        x, y, z = positions[i]
+        m = masses[i]
+
+        I11 += m * (y**2 + z**2)
+        I22 += m * (x**2 + z**2)
+        I33 += m * (x**2 + y**2)
+        I12 += -m * x * y
+        I13 += -m * x * z
+        I23 += -m * y * z
+
+    I = np.array([[I11, I12, I13], [I12, I22, I23], [I13, I23, I33]])
+
+    evals, evecs = np.linalg.eigh(I)
+    return evals
+
+
+class IdealGasThermo:
+    """import from ase.thermochemistry.IdealGasThermo
+
+    Parameters
+    ----------
+    vib_energies : list
+        List of vibrational energies in eV.
+    geometry : str
+        One of 'linear', 'nonlinear', 'monatomic'
+    potentialenergy : float
+        Potential energy in eV.
+    elements : list
+        such as ['H', 'O'].
+    symmetrynumber : int
+        Symmetry number.
+    spin : int
+        Spin multiplicity.
+    natoms : int
+        Number of atoms.
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import IdealGasThermo
+    >>> thermo = IdealGasThermo(vib_energies=[0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
+    ...                         geometry='linear', potentialenergy=0.,  # eV
+    ...                         elements=['H', 'O'], positions=[[0, 0, 0], [0, 0, 1]],  # angstrom
+    ...                         symmetrynumber=None, spin=None, natoms=None)
+    >>> thermo.get_enthalpy(298.15)  # K
+    Enthalpy components at T = 298.15 K:
+    ===============================
+    E_pot                  0.000 eV
+    E_ZPE                  0.300 eV
+    Cv_trans (0->T)        0.039 eV
+    Cv_rot (0->T)          0.026 eV
+    Cv_vib (0->T)          0.000 eV
+    (C_v -> C_p)           0.026 eV
+    -------------------------------
+    H                      0.390 eV
+    ===============================
+    0.389924026967057
+    """
+
+    # 读取elements数组代替atoms
+    def __init__(
+        self,
+        vib_energies,
+        geometry,
+        potentialenergy=0.0,
+        elements=None,
+        positions=None,
+        symmetrynumber=None,
+        spin=None,
+        natoms=None,
+    ):
+        self.potentialenergy = potentialenergy
+        self.geometry = geometry
+        self.elements = elements
+        if isinstance(positions, list):
+            self.positions = np.array(positions, dtype=float)
+        elif isinstance(positions, np.ndarray):
+            self.positions = positions
+        else:
+            raise TypeError("positions must be list or np.ndarray")
+        if isinstance(vib_energies, list):
+            vib_energies = np.array(vib_energies)
+        elif isinstance(vib_energies, np.ndarray):
+            pass
+        else:
+            raise TypeError("vib_energies must be list or np.ndarray")
+        self.sigma = symmetrynumber
+        self.spin = spin
+        if natoms is None:
+            if elements:
+                natoms = len(elements)
+        # Cut the vibrations to those needed from the geometry.
+        if natoms:
+            if geometry == "nonlinear":
+                self.vib_energies = vib_energies[-(3 * natoms - 6) :]
+            elif geometry == "linear":
+                self.vib_energies = vib_energies[-(3 * natoms - 5) :]
+            elif geometry == "monatomic":
+                self.vib_energies = []
+        else:
+            self.vib_energies = vib_energies
+        # Make sure no imaginary frequencies remain.
+        if sum(np.iscomplex(self.vib_energies)):
+            raise ValueError("Imaginary frequencies are present.")
+        else:
+            self.vib_energies = np.real(self.vib_energies)  # clear +0.j
+        self.referencepressure = 1.0e5  # Pa
+        self.natoms = natoms
+
+    def get_ZPE_correction(self):
+        """Returns the zero-point vibrational energy correction in eV."""
+        zpe = 0.0
+        for energy in self.vib_energies:
+            zpe += 0.5 * energy
+        return zpe
+
+    def _vibrational_energy_contribution(self, temperature):
+        """Calculates the change in internal energy due to vibrations from
+        0K to the specified temperature for a set of vibrations given in
+        eV and a temperature given in Kelvin. Returns the energy change
+        in eV."""
+        kT = k * temperature
+        dU = 0.0
+        for energy in self.vib_energies:
+            dU += energy / (np.exp(energy / kT) - 1.0)
+        return dU
+
+    def _vibrational_entropy_contribution(self, temperature):
+        """Calculates the entropy due to vibrations for a set of vibrations
+        given in eV and a temperature given in Kelvin.  Returns the entropy
+        in eV/K."""
+        kT = k * temperature
+        S_v = 0.0
+        for energy in self.vib_energies:
+            x = energy / kT
+            S_v += x / (np.exp(x) - 1.0) - np.log(1.0 - np.exp(-x))
+        S_v *= k
+        return S_v
+
+    def get_enthalpy(self, temperature):
+        """Returns the enthalpy, in eV, in the ideal gas approximation
+        at a specified temperature (K)."""
+
+        fmt = "%-15s%13.3f eV"
+        print("Enthalpy components at T = %.2f K:" % temperature)
+        print("=" * 31)
+
+        H = 0.0
+
+        print(fmt % ("E_pot", self.potentialenergy))
+        H += self.potentialenergy
+
+        zpe = self.get_ZPE_correction()
+        print(fmt % ("E_ZPE", zpe))
+        H += zpe
+
+        Cv_t = 3.0 / 2.0 * k  # translational heat capacity (3-d gas)
+        print(fmt % ("Cv_trans (0->T)", Cv_t * temperature))
+        H += Cv_t * temperature
+
+        if self.geometry == "nonlinear":  # rotational heat capacity
+            Cv_r = 3.0 / 2.0 * k
+        elif self.geometry == "linear":
+            Cv_r = k
+        elif self.geometry == "monatomic":
+            Cv_r = 0.0
+        print(fmt % ("Cv_rot (0->T)", Cv_r * temperature))
+        H += Cv_r * temperature
+
+        dH_v = self._vibrational_energy_contribution(temperature)
+        print(fmt % ("Cv_vib (0->T)", dH_v))
+        H += dH_v
+
+        Cp_corr = k * temperature
+        print(fmt % ("(C_v -> C_p)", Cp_corr))
+        H += Cp_corr
+
+        print("-" * 31)
+        print(fmt % ("H", H))
+        print("=" * 31)
+        return H
+
+    def get_entropy(self, temperature, pressure):
+        """Returns the entropy, in eV/K, in the ideal gas approximation
+        at a specified temperature (K) and pressure (Pa)."""
+
+        if self.elements is None or self.sigma is None or self.spin is None:
+            raise RuntimeError(
+                "elements, symmetrynumber, and spin must be "
+                "specified for entropy and free energy "
+                "calculations."
+            )
+        S = 0.0
+        # Translational entropy (term inside the log is in SI units).
+        mass = sum(eles2masses(self.elements)) * amu  # kg/molecule
+        S_t = (2 * np.pi * mass * kB * temperature / h**2) ** (3.0 / 2)
+        S_t *= kB * temperature / self.referencepressure
+        S_t = k * (np.log(S_t) + 5.0 / 2.0)
+        S += S_t
+
+        # Rotational entropy (term inside the log is in SI units).
+        if self.geometry == "monatomic":
+            S_r = 0.0
+        elif self.geometry == "nonlinear":
+            inertias = (
+                get_ma(self.elements, self.positions, self.natoms)
+                * amu
+                / (10.0**10) ** 2
+            )  # kg m^2
+            S_r = np.sqrt(np.pi * np.product(inertias)) / self.sigma
+            S_r *= (8.0 * np.pi**2 * kB * temperature / h**2) ** (3.0 / 2.0)
+            S_r = k * (np.log(S_r) + 3.0 / 2.0)
+        elif self.geometry == "linear":
+            inertias = (
+                get_ma(self.elements, self.positions, self.natoms)
+                * amu
+                / (10.0**10) ** 2
+            )  # kg m^2
+            inertia = max(inertias)  # should be two identical and one zero
+            S_r = 8 * np.pi**2 * inertia * kB * temperature / self.sigma / h**2
+            S_r = k * (np.log(S_r) + 1.0)
+        S += S_r
+        # Electronic entropy.
+        S_e = k * np.log(2 * self.spin + 1)
+        S += S_e
+        # Vibrational entropy.
+        S_v = self._vibrational_entropy_contribution(temperature)
+        S += S_v
+        # Pressure correction to translational entropy.
+        S_p = -k * np.log(pressure / self.referencepressure)
+        S += S_p
+        return S
+
+    def get_gibbs_energy(self, temperature, pressure):
+        """Returns the Gibbs free energy, in eV, in the ideal gas
+        approximation at a specified temperature (K) and pressure (Pa)."""
+
+        H = self.get_enthalpy(temperature)
+        print("")
+        S = self.get_entropy(temperature, pressure)
+        G = H - temperature * S
+
+        print("")
+        print(
+            "Free energy components at T = %.2f K and P = %.1f Pa:"
+            % (temperature, pressure)
+        )
+        print("=" * 23)
+        fmt = "%5s%15.3f eV"
+        print(fmt % ("H", H))
+        print(fmt % ("-T*S", -temperature * S))
+        print("-" * 23)
+        print(fmt % ("G", G))
+        print("=" * 23)
+        return G
+
+
+def getTSgas(
+    fretxt="frequency.txt",
+    datafile=".",
+    potentialenergy=0,  # eV
+    elements=None,
+    geometry="linear",
+    positions=None,  # Angstrom
+    symmetrynumber=1,
+    spin=1,
+    temperature=298.15,
+    pressure=101325,
+):
+    """理想气体近似下，计算熵的能量贡献
+
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    datafile : str
+        计算结果json或h5文件或包含它们的文件夹路径, 默认当前路径；
+        如果设置为None，则需要传入elements和positions参数
+    potentialenergy : float
+        势能，单位eV
+    elements : list
+        元素列表，如果
+    geometry : str
+        分子几何，monatomic, linear, nonlinear
+    positions : list
+        原子坐标，单位Angstrom
+    symmetrynumber : int
+        对称数
+    spin : int
+        自旋数
+    temperature : float
+        温度，单位K
+    pressure : float
+        压强，单位Pa
+
+    Returns
+    -------
+    TSgas : float
+        理想气体近似下，计算熵的能量贡献，单位eV
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import getTSgas
+    >>> TSgas = getTSgas(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', datafile='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.h5', potentialenergy=-0.0,  geometry='linear', symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
+    >>> print(TSgas)
+    0.8515317035550232
+    >>> TSgas = getTSgas(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', datafile='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.h5', potentialenergy=-0.0,  geometry='linear', symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
+    >>> TSgas
+    0.8515317035550232
+    """
+    ve = []
+    with open(fretxt) as ft:
+        lines = ft.readlines()
+        for i in range(2, len(lines)):
+            if lines[i].strip()[1] == "f/i":
+                ve.append(complex(lines[i].split()[-1]) / 1000)
+            else:
+                ve.append(float(lines[i].split()[-1]) / 1000)
+
+    if datafile:  # skip if datafile is None
+        # search datafile in the given directory
+        if os.path.isdir(datafile):
+            directory = datafile  # specified datafile is actually a directory
+            print("您指定了一个文件夹，正在查找相关h5或json文件...")
+            if os.path.exists(os.path.join(directory, "frequency.h5")):
+                datafile = os.path.join(directory, "frequency.h5")
+                print("Reading frequency.h5...")
+            elif os.path.exists(os.path.join(directory, "frequency.json")):
+                datafile = os.path.join(directory, "frequency.json")
+                print("Reading frequency.json...")
+            else:
+                raise FileNotFoundError("未找到frequency.h5/frequency.json文件！")
+        if datafile.endswith(".h5"):
+            eles = get_ele_from_h5(datafile)
+            import h5py
+
+            data = h5py.File(datafile)
+            poses = np.array(data.get("/AtomInfo/Position")).reshape(-1, 3)
+
+        elif datafile.endswith(".json"):
+            import json
+
+            with open(datafile) as f:
+                data = json.load(f)
+            atoms = data["AtomInfo"]["Atoms"]
+            eles = []
+            poses = []
+            for i in range(len(atoms)):
+                eles.append(atoms[i]["Element"])
+                poses.append(atoms[i]["Position"])
+        else:
+            raise TypeError("仅支持读取h5或json文件！")
+    else:
+        eles = elements
+        poses = positions
+
+    # 计算熵的能量贡献
+    thermo = IdealGasThermo(
+        vib_energies=ve,  # eV
+        potentialenergy=potentialenergy,  # eV
+        elements=eles,
+        geometry=geometry,
+        positions=poses,  # Angstrom
+        symmetrynumber=symmetrynumber,
+        spin=spin,
+    )
+    S = thermo.get_entropy(temperature, pressure)
+
+    return S * temperature
+
+
+def d_band(spin, dos_data: CompleteDos):  # 定义函数，括号里给出函数的两个变量
+    """计算d带中心
+
+    Parameters
+    ----------
+    spin : Spin.up或Spin.down
+        自旋类型，
+    dos_data : pymatgen.electronic_structure.dos.CompleteDos
+        dos数据
+
+    Returns
+    -------
+    db1 : float
+        d带中心数值
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import d_band
+    >>> from dspawpy.io.read import get_dos_data
+    >>> dos_data = get_dos_data("/data/home/hzw1002/dspawpy_repo/test/supplement/dos.h5")  # 从dos.h5中读取数据
+    >>> for spin in dos_data.densities:
+    ...     print('spin=', spin)
+    ...     c = d_band(spin, dos_data)
+    ...     print(c)
+    spin= 1
+    -3.666508748164936
+    """
+    dos_d = dos_data.get_spd_dos()[OrbitalType.d]
+    # dos_d = dos_data.get_spd_dos()[d]
+    Efermi = dos_data.efermi
+    epsilon = dos_d.energies - Efermi  # shift d-band center
+
+    N1 = dos_d.densities[spin]
+    M1 = epsilon * N1
+    SummaM1 = integrate.simps(M1, epsilon)
+    SummaN1 = integrate.simps(N1, epsilon)
+
+    return SummaM1 / SummaN1
+
+
+def getZPE(fretxt: str = "frequency.txt"):
+    """从fretext中读取数据，计算ZPE
+
+    将另外保存结果到 ZPE_TS.dat 中
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+
+    Returns
+    -------
+    ZPE: float
+        零点能
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import getZPE
+    >>> ZPE= getZPE(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt')
+    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
+       Frequency (meV)
+    0       284.840033
+    <BLANKLINE>
+    正在写入ZPE.dat文件...
+    <BLANKLINE>
+    --> Zero-point energy,  ZPE (eV): 0.1424200165
+    >>> ZPE
+    0.1424200165
+    """
+
+    # 1. read data
+    data_get_ZPE = []
+    with open(fretxt, "r") as f:
+        for line in f.readlines():
+            data_line = line.strip().split()
+            if len(data_line) != 6:
+                continue
+            if data_line[1] == "f":
+                data_get_ZPE.append(float(data_line[5]))
+
+    data_get_ZPE = np.array(data_get_ZPE)
+
+    # 2. printout to check
+    print(f"=== 从{fretxt}中读取到的相关如下 ===")
+    dt = pd.DataFrame({"Frequency (meV)": data_get_ZPE}, index=None)
+    print(dt)
+
+    if len(data_get_ZPE) == 0:
+        raise ValueError("全是虚频，请考虑重新优化结构...")
+    else:
+        print("\n正在写入ZPE.dat文件...")
+        np.savetxt(
+            "ZPE.dat",
+            np.array(data_get_ZPE).T,
+            fmt="%.6f",
+            header="Frequency (meV)",
+            comments=f"Data read from {os.path.abspath(fretxt)}\n",
+        )
+
+    # 3. calculate
+    ZPE = 0
+    for data in data_get_ZPE:
+        ZPE += data / 2000.0
+    print("\n--> Zero-point energy,  ZPE (eV):", ZPE)
+
+    with open("ZPE.dat", "a") as f:
+        f.write(f"\n--> Zero-point energy,  ZPE (eV): {ZPE}")
+
+    return ZPE
+
+
+def getTSads(fretxt: str = "frequency.txt", T: float = 298.15):
+    """从fretext中读取数据，计算ZPE和TS
+
+    将另外保存结果到 ZPE_TS.dat 中
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    T : float
+        温度，单位K, 默认298.15
+
+    Returns
+    -------
+    TS: float
+        熵校正
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import getTSads
+    >>> TS = getTSads(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', T=298.15)
+    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
+       Frequency (THz)
+    0        68.873993
+    <BLANKLINE>
+    正在写入TS.dat文件...
+    --> Entropy contribution, T*S (eV)： 4.7566997225177686e-06
+    >>> TS
+    4.7566997225177686e-06
+    """
+    data_get_TS = []
+    with open(fretxt, "r") as f:
+        for line in f.readlines():
+            data_line = line.strip().split()
+            if len(data_line) != 6:
+                continue
+            if data_line[1] == "f":
+                data_get_TS.append(float(data_line[2]))
+
+    data_get_TS = np.array(data_get_TS)
+
+    # 2. printout to check
+    print(f"=== 从{fretxt}中读取到的相关如下 ===")
+    dt = pd.DataFrame({"Frequency (THz)": data_get_TS}, index=None)
+    print(dt)
+
+    if len(data_get_TS) == 0:
+        raise ValueError("全是虚频，请考虑重新优化结构...")
+    else:
+        print("\n正在写入TS.dat文件...")
+        np.savetxt(
+            "TS.dat",
+            np.array(data_get_TS).T,
+            fmt="%.6f",
+            header="Frequency (THz)",
+            comments=f"Data read from {os.path.abspath(fretxt)}\n",
+        )
+
+    # 3. calculate
+    sum_S = 0
+    import math  # 因为要使用 e的多少次方，ln（）对数
+
+    for vi_THz in data_get_TS:
+        vi_Hz = vi_THz * 1e12
+        m1 = h * Na * vi_Hz
+        m2 = h * vi_Hz / (kB * T)
+        m3 = math.exp(m2) - 1
+        m4 = T * m3
+        m5 = 1 - math.exp(-m2)  # math.exp(3) 就是e的3次方
+        m6 = math.log(m5, math.e)  # m6= ln(m5)   math.e在python中=e ，以右边为底的对数
+        m7 = R * m6
+        m8 = m1 / m4 - m7  # S 单位J/(mol*K)
+        m9 = (T * m8 / 1000) / 96.49  # T*S,将单位化为KJ/mol, 96.49 kJ/mol = 1 eV 单位eV
+        sum_S += m9
+
+    print("--> Entropy contribution, T*S (eV)：", sum_S)
+
+    with open("ZPE_TS.dat", "a") as f:
+        f.write(f"\n--> Entropy contribution, T*S (eV): {sum_S}\n")
+
+    return sum_S
+
+
+def thermo_correction(fretxt: str = "frequency.txt", T: float = 298.15):
+    """从fretext中读取数据，计算ZPE和TS
+    将另外保存结果到 ZPE_TS.dat 中
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    T : float
+        温度，单位K, 默认298.15
+
+    Returns
+    -------
+    ZPE: float
+        零点能
+    TS: float
+        熵校正
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import thermo_correction
+    >>> ZPE, TS = thermo_correction(fretxt='/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt', T=298.15)
+    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
+       Frequency (meV)
+    0       284.840033
+    <BLANKLINE>
+    正在写入ZPE.dat文件...
+    <BLANKLINE>
+    --> Zero-point energy,  ZPE (eV): 0.1424200165
+    === 从/data/home/hzw1002/dspawpy_repo/test/2.13/frequency.txt中读取到的相关如下 ===
+       Frequency (THz)
+    0        68.873993
+    <BLANKLINE>
+    正在写入TS.dat文件...
+    --> Entropy contribution, T*S (eV)： 4.7566997225177686e-06
+    >>> ZPE
+    0.1424200165
+    >>> TS
+    4.7566997225177686e-06
+    """
+
+    ZPE = getZPE(fretxt=fretxt)
+    sum_S = getTSads(fretxt=fretxt, T=T)
+
+    return ZPE, sum_S
+
+
+def _symbols2numbers(symbols) -> List[int]:
+    numbers = []
+    for s in symbols:
+        if isinstance(s, str):
+            numbers.append(atomic_numbers[s])
+        else:
+            numbers.append(int(s))
+    return numbers
```

## dspawpy/io/write.py

```diff
@@ -1,765 +1,763 @@
-"""
-Functions to write files
-"""
-
-import json
-import os
-
-import numpy as np
-from pymatgen.core.structure import Structure
-
-from dspawpy.io.read import _get_lammps_non_orthogonal_box, load_h5
-
-
-def _write_xyz_traj(
-    structures,
-    xyzfile="aimdTraj.xyz",
-):
-    r"""保存xyz格式的轨迹文件
-
-    Parameters
-    ----------
-    structures: list
-        pymatgen的Structures列表
-    xyzfile : str
-        写入xyz格式的轨迹文件，默认为aimdTraj.xyz
-    """
-    if not isinstance(structures, list):  # single Structure
-        structures = [structures]
-    if os.path.isfile(xyzfile):
-        print("Warning: %s already exists and will be overwritten!" % xyzfile)
-    if os.path.dirname(xyzfile) != "":
-        os.makedirs(os.path.dirname(xyzfile), exist_ok=True)
-    with open(xyzfile, "w") as f:
-        # Nstep
-        for _, structure in enumerate(structures):
-            # 原子数不会变，就是不合并的元素总数
-            eles = [s.species_string for s in structure.sites]
-            f.write("%d\n" % len(eles))
-            # lattice
-            lm = structure.lattice.matrix
-            f.write(
-                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
-                % (
-                    lm[0, 0],
-                    lm[0, 1],
-                    lm[0, 2],
-                    lm[1, 0],
-                    lm[1, 1],
-                    lm[1, 2],
-                    lm[2, 0],
-                    lm[2, 1],
-                    lm[2, 2],
-                )
-            )
-            # position and element
-            poses = structure.cart_coords
-            for j in range(len(eles)):
-                f.write(
-                    "%s %f %f %f\n" % (eles[j], poses[j, 0], poses[j, 1], poses[j, 2])
-                )
-
-    print(f"{xyzfile} 文件已保存！")
-
-
-def _write_dump_traj(
-    structures,
-    dumpfile="aimdTraj.dump",
-):
-    r"""保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
-
-    Parameters
-    ----------
-    structures: list
-        pymatgen的Structures列表
-    dumpfile : str
-        dump格式的轨迹文件名，默认为aimdTraj.dump
-    """
-    if not isinstance(structures, list):  # single Structure
-        structures = [structures]
-    if os.path.isfile(dumpfile):
-        print("Warning: %s already exists and will be overwritten!" % dumpfile)
-    if os.path.dirname(dumpfile) != "":
-        os.makedirs(os.path.dirname(dumpfile), exist_ok=True)
-    with open(dumpfile, "w") as f:
-        for n, structure in enumerate(structures):
-            lat = structure.lattice.matrix
-            eles = [s.species_string for s in structure.sites]
-            poses = structure.cart_coords
-
-            box_bounds = _get_lammps_non_orthogonal_box(lat)
-            f.write("ITEM: TIMESTEP\n%d\n" % n)
-            f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
-            f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
-            f.write(
-                "%f %f %f\n%f %f %f\n %f %f %f\n"
-                % (
-                    box_bounds[0][0],
-                    box_bounds[0][1],
-                    box_bounds[0][2],
-                    box_bounds[1][0],
-                    box_bounds[1][1],
-                    box_bounds[1][2],
-                    box_bounds[2][0],
-                    box_bounds[2][1],
-                    box_bounds[2][2],
-                )
-            )
-            f.write("ITEM: ATOMS type x y z id\n")
-            for i in range(len(eles)):
-                f.write(
-                    "%s %f %f %f %d\n"
-                    % (
-                        eles[i],
-                        poses[i, 0],
-                        poses[i, 1],
-                        poses[i, 2],
-                        i + 1,
-                    )
-                )
-    print(f"{dumpfile} 文件已保存！")
-
-
-def write_VESTA(in_filename: str, data_type, out_filename="DS-PAW.vesta"):
-    """从包含电子体系信息的json或h5文件中读取数据并写入VESTA格式的文件中
-
-    Parameters
-    ----------
-    in_filename : str
-        包含电子体系信息的json或h5文件路径
-    data_type: str
-        数据类型，支持 "rho", "potential", "elf", "pcharge", "boundcharge"
-    out_filename : str
-        输出文件路径, 默认 "DS-PAW.vesta"
-
-    Returns
-    --------
-    out_filename : file
-        VESTA格式的文件
-
-    Examples
-    --------
-    >>> from dspawpy.io.write import write_VESTA
-    >>> write_VESTA("/data/home/hzw1002/dspawpy_repo/test/2.2/rho.json", "rho", out_filename='/data/home/hzw1002/dspawpy_repo/test/out/rho.json')
-    """
-    if in_filename.endswith(".h5"):
-        data = load_h5(in_filename)
-        if data_type.lower() == "rho" or data_type.lower() == "boundcharge":
-            _write_VESTA_format(data, ["/Rho/TotalCharge"], out_filename)
-        elif data_type.lower() == "potential":
-            _write_VESTA_format(
-                data,
-                [
-                    "/Potential/TotalElectrostaticPotential",
-                ],
-                out_filename,
-            )
-        elif data_type.lower() == "elf":
-            _write_VESTA_format(data, ["/ELF/TotalELF"], out_filename)
-        elif data_type.lower() == "pcharge":
-            _write_VESTA_format(data, ["/Pcharge/1/TotalCharge"], out_filename)
-        else:
-            raise NotImplementedError("仅支持rho/potential/elf/pcharge/boundcharge")
-
-    elif in_filename.endswith(".json"):
-        with open(in_filename, "r") as fin:
-            data = json.load(fin)
-        if data_type.lower() == "rho" or data_type.lower() == "boundcharge":
-            _write_VESTA_format_json(
-                data["AtomInfo"], [data["Rho"]["TotalCharge"]], out_filename
-            )
-        elif data_type.lower() == "potential":
-            _write_VESTA_format_json(
-                data["AtomInfo"],
-                [
-                    data["Potential"]["TotalElectrostaticPotential"],
-                ],
-                out_filename,
-            )
-        elif data_type.lower() == "elf":
-            _write_VESTA_format_json(
-                data["AtomInfo"], [data["ELF"]["TotalELF"]], out_filename
-            )
-        elif data_type.lower() == "pcharge":
-            _write_VESTA_format_json(
-                data["AtomInfo"], [data["Pcharge"][0]["TotalCharge"]], out_filename
-            )
-        else:
-            raise NotImplementedError("仅支持rho/potential/elf/pcharge/boundcharge")
-
-    else:
-        raise NotImplementedError("仅支持json或h5格式文件")
-
-
-def write_delta_rho_vesta(AB, A, B, output="delta_rho.vesta"):
-    """电荷密度差分可视化
-
-    DeviceStudio暂不支持大文件，临时写成可以用VESTA打开的格式
-
-    Parameters
-    ----------
-    AB : str
-        AB的电荷密度文件路径，可以是h5或json格式
-    A : str
-        A的电荷密度文件路径，可以是h5或json格式
-    B : str
-        B的电荷密度文件路径，可以是h5或json格式
-    output : str
-        输出文件路径，默认 "delta_rho.vesta"
-
-    Returns
-    -------
-    output : file
-        电荷差分（AB-A-B）后的电荷密度文件，
-
-    Examples
-    --------
-    >>> from dspawpy.io.write import write_delta_rho_vesta
-    >>> write_delta_rho_vesta('/data/home/hzw1002/dspawpy_repo/test/supplement/AB.h5', '/data/home/hzw1002/dspawpy_repo/test/supplement/A.h5', '/data/home/hzw1002/dspawpy_repo/test/supplement/B.h5', '/data/home/hzw1002/dspawpy_repo/test/out/delta_rho.vesta')
-    读取/data/home/hzw1002/dspawpy_repo/test/supplement/AB.h5...
-    读取/data/home/hzw1002/dspawpy_repo/test/supplement/A.h5...
-    读取/data/home/hzw1002/dspawpy_repo/test/supplement/B.h5...
-    计算电荷差分...
-    写入文件/data/home/hzw1002/dspawpy_repo/test/out/delta_rho.vesta...
-    成功写入 /data/home/hzw1002/dspawpy_repo/test/out/delta_rho.vesta
-    """
-    print(f"读取{AB}...")
-    if AB.endswith(".h5"):
-        dataAB = load_h5(AB)
-        rhoAB = np.array(dataAB["/Rho/TotalCharge"])
-        nGrids = dataAB["/AtomInfo/Grid"]
-        atom_symbol = dataAB["/AtomInfo/Elements"]
-        atom_pos = dataAB["/AtomInfo/Position"]
-        latticeConstantMatrix = dataAB["/AtomInfo/Lattice"]
-        atom_pos = np.array(atom_pos).reshape(-1, 3)
-    elif AB.endswith(".json"):
-        atom_symbol = []
-        atom_pos = []
-        with open(AB, "r") as f1:
-            dataAB = json.load(f1)
-            rhoAB = np.array(dataAB["Rho"]["TotalCharge"])
-            nGrids = dataAB["AtomInfo"]["Grid"]
-        for i in range(len(dataAB["AtomInfo"]["Atoms"])):
-            atom_symbol.append(dataAB["AtomInfo"]["Atoms"][i]["Element"])
-            atom_pos.append(dataAB["AtomInfo"]["Atoms"][i]["Position"])
-        atom_pos = np.array(atom_pos)
-
-        latticeConstantMatrix = dataAB["AtomInfo"]["Lattice"]
-    else:
-        raise ValueError(f"file format must be either h5 or json: {AB}")
-
-    print(f"读取{A}...")
-    if A.endswith(".h5"):
-        dataA = load_h5(A)
-        rhoA = np.array(dataA["/Rho/TotalCharge"])
-    elif A.endswith(".json"):
-        with open(A, "r") as f2:
-            dataA = json.load(f2)
-            rhoA = np.array(dataA["Rho"]["TotalCharge"])
-    else:
-        raise ValueError(f"file format must be either h5 or json: {A}")
-
-    print(f"读取{B}...")
-    if B.endswith(".h5"):
-        dataB = load_h5(B)
-        rhoB = np.array(dataB["/Rho/TotalCharge"])
-    elif B.endswith(".json"):
-        with open(B, "r") as f3:
-            dataB = json.load(f3)
-            rhoB = np.array(dataB["Rho"]["TotalCharge"])
-    else:
-        raise ValueError(f"file format must be either h5 or json: {B}")
-
-    print(f"计算电荷差分...")
-    rho = rhoAB - rhoA - rhoB
-    rho = np.array(rho).reshape(nGrids[0], nGrids[1], nGrids[2])
-    element = list(set(atom_symbol))
-    element = sorted(set(atom_symbol), key=atom_symbol.index)
-    element_num = np.zeros(len(element))
-    for i in range(len(element)):
-        element_num[i] = atom_symbol.count(element[i])
-
-    latticeConstantMatrix = np.array(latticeConstantMatrix)
-    latticeConstantMatrix = latticeConstantMatrix.reshape(3, 3)
-
-    print(f"写入文件{output}...")
-    if os.path.isfile(output):
-        print("Warning: %s already exists and will be overwritten!" % output)
-    if os.path.dirname(output) != "":
-        os.makedirs(os.path.dirname(output), exist_ok=True)
-    with open(output, "w") as out:
-        out.write("DS-PAW_rho\n")
-        out.write("    1.000000\n")
-        for i in range(3):
-            for j in range(3):
-                out.write("    " + str(latticeConstantMatrix[i, j]) + "    ")
-            out.write("\n")
-        for i in range(len(element)):
-            out.write("    " + element[i] + "    ")
-        out.write("\n")
-
-        for i in range(len(element_num)):
-            out.write("    " + str(int(element_num[i])) + "    ")
-        out.write("\n")
-        out.write("Direct\n")
-        for i in range(len(atom_pos)):
-            for j in range(3):
-                out.write("    " + str(atom_pos[i, j]) + "    ")
-            out.write("\n")
-        out.write("\n")
-
-        for i in range(3):
-            out.write("  " + str(nGrids[i]) + "  ")
-        out.write("\n")
-
-        ind = 0
-        for i in range(nGrids[0]):
-            for j in range(nGrids[1]):
-                for k in range(nGrids[2]):
-                    out.write("  " + str(rho[i, j, k]) + "  ")
-                    ind = ind + 1
-                    if ind % 5 == 0:
-                        out.write("\n")
-
-    print(f"成功写入 {output}")
-
-
-def to_file(structure, filename: str, fmt=None, coords_are_cartesian=True, si=None):
-    r"""往结构文件中写入信息
-
-    Parameters
-    ----------
-    structure : Structure
-        pymatgen的Structure对象
-    filename : str
-        结构文件名
-    fmt : str
-        - 结构文件类型，原生支持 'json', 'as', 'hzw', 'pdb', 'xyz', 'dump' 六种，具体匹配规则见http://hzwtech.com/Device%20Studio/DS-PAW/build/html/tools.html#structure 8.2节表格
-        - 'pdb', 'xyz' 和 'dump' 支持传入多个结构，structure参数可以是一个Structure对象列表；其他类型的文件只支持传入单个结构
-    coords_are_cartesian : bool
-        - 是否写作笛卡尔坐标，默认为True；否则写成分数坐标形式
-        - 此选项暂时仅对 as 和 json 格式有效
-    si : int
-        结构编号索引
-
-    Examples
-    --------
-
-    先读取结构信息:
-
-    >>> from dspawpy.io.structure import build_Structures_from_datafile
-    >>> s = build_Structures_from_datafile('/data/home/hzw1002/dspawpy_repo/test/2.15/01/neb01.h5')
-    Reading /data/home/hzw1002/dspawpy_repo/test/2.15/01/neb01.h5...
-    >>> len(s)
-    17
-
-    将结构信息写入文件：
-
-    >>> from dspawpy.io.write import to_file
-    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.json', coords_are_cartesian=True)
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.json
-    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.as', coords_are_cartesian=True)
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.as
-    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.hzw', coords_are_cartesian=True)
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.hzw
-    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.pdb', coords_are_cartesian=True)
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.pdb
-    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.xyz', coords_are_cartesian=True)
-    /data/home/hzw1002/dspawpy_repo/test/out/PtH.xyz 文件已保存！
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.xyz
-    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.dump', coords_are_cartesian=True)
-    /data/home/hzw1002/dspawpy_repo/test/out/PtH.dump 文件已保存！
-    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.dump
-
-    单结构信息推荐使用 as 格式存储，如果 Structure 中有磁矩或自由度信息，将会按最完整的格式统一写入，形如 Fix_x, Fix_y, Fix_z, Mag_x, Mag_y, Mag_z，自由度信息默认为 F，磁矩默认为 0.0。可视情况自行手动删除生成的 as 文件中的这些默认信息
-
-    >>> with open('/data/home/hzw1002/dspawpy_repo/test/out/PtH.as') as f:
-    ...     print(f.read())
-    ...
-    Total number of atoms
-    13
-    Lattice Fix_x Fix_y Fix_z
-     5.60580000 0.00000000 0.00000000 F F F
-     0.00000000 5.60580000 0.00000000 F F F
-     0.00000000 0.00000000 16.81740000 F F F
-    Cartesian Fix_x Fix_y Fix_z Mag
-    H 2.58985263 3.72755271 6.94246998 F F F 0.0
-    Pt 1.37942121 1.39655502 1.96304099 F F F 0.0
-    Pt 4.20055071 1.40326436 1.94681875 F F F 0.0
-    Pt 1.37462277 4.20932677 2.00221003 F F F 0.0
-    Pt 4.21197615 4.21324064 1.99578112 F F F 0.0
-    Pt 5.58740047 5.59517338 3.93274445 F F F 0.0
-    Pt 5.58633749 2.78068345 3.91301343 F F F 0.0
-    Pt 2.79076605 5.59305895 3.91208092 F F F 0.0
-    Pt 2.78904685 2.78501463 3.89610696 F F F 0.0
-    Pt 1.38102265 1.36691874 5.84326681 F F F 0.0
-    Pt 4.19057728 1.36788897 5.84877666 F F F 0.0
-    Pt 1.34667410 4.16198043 5.89298591 F F F 0.0
-    Pt 4.17046728 4.15729941 5.89874209 F F F 0.0
-    <BLANKLINE>
-
-    写成 json / hzw/ pdb 文件，将忽略磁矩和自由度信息
-    """
-    if si is not None:
-        assert isinstance(si, int), "si 应当是用于索引列表的整数"
-    if isinstance(structure, Structure):
-        structure = [structure]
-
-    if fmt is None:
-        fmt = filename.split(".")[-1]
-
-    if fmt == "pdb":  # 可以是多个构型
-        if si:
-            _to_pdb(structure[si], filename)
-        else:
-            _to_pdb(structure, filename)
-    elif fmt == "xyz":  # 可以是多个构型
-        if si:
-            _write_xyz_traj(structure[si], filename)
-        else:
-            _write_xyz_traj(structure, filename)
-    elif fmt == "dump":  # 可以是多个构型
-        if si:
-            _write_dump_traj(structure[si], filename)
-        else:
-            _write_dump_traj(structure, filename)
-
-    elif fmt == "json":  # 单个构型
-        if si:
-            _to_dspaw_json(structure[si], filename, coords_are_cartesian)
-        else:
-            _to_dspaw_json(structure[-1], filename, coords_are_cartesian)
-    elif fmt == "as":
-        if si:
-            _to_dspaw_as(structure[si], filename, coords_are_cartesian)
-        else:
-            _to_dspaw_as(structure[-1], filename, coords_are_cartesian)
-    elif fmt == "hzw":
-        if si:
-            _to_hzw(structure[si], filename)
-        else:
-            _to_hzw(structure[-1], filename)
-
-    elif fmt in [
-        "cif",
-        "mcif",
-        "poscar",
-        "cssr",
-        "xsf",
-        "mcsqs",
-        "yaml",
-        "fleur-inpgen",
-        "prismatic",
-        "res",
-    ]:
-        if si:
-            structure[si].to(filename, fmt=fmt)
-        else:
-            structure[-1].to(filename, fmt=fmt)
-
-    else:
-        try:
-            if si:
-                structure[si].to(filename)
-            else:
-                structure[-1].to(filename)
-        except Exception as e:
-            raise NotImplementedError(
-                f"除了 pdb, xyz, dump, json, as, hzw 六种格式外，其他格式一律移交 pymatgen 处理，然而\n--> pymatgen返回错误：{e}"
-            )
-
-    print(f"--> 成功写入文件 {os.path.abspath(filename)}")
-
-
-def _write_atoms(fileobj, hdf5):
-    fileobj.write("DS-PAW Structure\n")
-    fileobj.write("  1.00\n")
-    lattice = np.asarray(hdf5["/AtomInfo/Lattice"]).reshape(-1, 1)  # 将列表lattice下的多个列表整合
-    fileobj.write(
-        "%10.6f %10.6f %10.6f\n" % (lattice[0][0], lattice[1][0], lattice[2][0])
-    )
-    fileobj.write(
-        "%10.6f %10.6f %10.6f\n" % (lattice[3][0], lattice[4][0], lattice[5][0])
-    )
-    fileobj.write(
-        "%10.6f %10.6f %10.6f\n" % (lattice[6][0], lattice[7][0], lattice[8][0])
-    )
-
-    elements = hdf5["/AtomInfo/Elements"]
-    elements_set = []
-    elements_number = {}
-    for e in elements:
-        if e in elements_set:
-            elements_number[e] = elements_number[e] + 1
-        else:
-            elements_set.append(e)
-            elements_number[e] = 1
-
-    for e in elements_set:
-        fileobj.write("  " + e)
-    fileobj.write("\n")
-
-    for e in elements_set:
-        fileobj.write("%5d" % (elements_number[e]))
-    fileobj.write("\n")
-    if hdf5["/AtomInfo/CoordinateType"][0] == "Direct":
-        fileobj.write("Direct\n")
-    else:
-        fileobj.write("Cartesian\n")
-    for i, p in enumerate(hdf5["/AtomInfo/Position"]):
-        fileobj.write("%10.6f" % p)
-        if (i + 1) % 3 == 0:
-            fileobj.write("\n")
-    fileobj.write("\n")
-
-
-def _write_VESTA_format(hdf5: dict, datakeys: list, filename):
-    if os.path.isfile(filename):
-        print("Warning: %s already exists and will be overwritten!" % filename)
-    if os.path.dirname(filename) != "":
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-    with open(filename, "w") as file:
-        _write_atoms(file, hdf5)
-        for key in datakeys:
-            d = np.asarray(hdf5[key]).reshape(-1, 1)  # 将列表hdf5[key]下的多个列表整合
-            file.write("%5d %5d %5d\n" % tuple(hdf5["/AtomInfo/Grid"]))
-            i = 0
-            while i < len(d):
-                for j in range(10):
-                    file.write("%10.5f " % d[i])
-                    i += 1
-                    if i >= len(d):
-                        break
-                file.write("\n")
-
-            file.write("\n")
-
-
-def _write_atoms_json(fileobj, atom_info):
-    fileobj.write("DS-PAW Structure\n")
-    fileobj.write("  1.00\n")
-    lattice = atom_info["Lattice"]
-
-    fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[0], lattice[1], lattice[2]))
-    fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[3], lattice[4], lattice[5]))
-    fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[6], lattice[7], lattice[8]))
-
-    elements = [atom["Element"] for atom in atom_info["Atoms"]]
-    elements_set = []
-    elements_number = {}
-    for e in elements:
-        if e in elements_set:
-            elements_number[e] = elements_number[e] + 1
-        else:
-            elements_set.append(e)
-            elements_number[e] = 1
-
-    for e in elements_set:
-        fileobj.write("  " + e)
-    fileobj.write("\n")
-
-    for e in elements_set:
-        fileobj.write("%5d" % (elements_number[e]))
-    fileobj.write("\n")
-    if atom_info["CoordinateType"] == "Direct":
-        fileobj.write("Direct\n")
-    else:
-        fileobj.write("Cartesian\n")
-    for atom in atom_info["Atoms"]:
-        fileobj.write("%10.6f %10.6f %10.6f\n" % tuple(atom["Position"]))
-    fileobj.write("\n")
-
-
-def _write_VESTA_format_json(atom_info: dict, data: list, filename):
-    if os.path.isfile(filename):
-        print("Warning: %s already exists and will be overwritten!" % filename)
-    if os.path.dirname(filename) != "":
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-    with open(filename, "w") as file:
-        _write_atoms_json(file, atom_info)
-        for d in data:
-            file.write("%5d %5d %5d\n" % tuple(atom_info["Grid"]))
-            i = 0
-            while i < len(d):
-                for j in range(10):
-                    file.write("%10.5f " % d[i])
-                    i += 1
-                    if i >= len(d):
-                        break
-                file.write("\n")
-
-            file.write("\n")
-
-
-def _to_dspaw_as(structure, filename: str, coords_are_cartesian=True):
-    """write dspaw structure file of .as type"""
-    if os.path.isfile(filename):
-        print("Warning: %s already exists and will be overwritten!" % filename)
-    if os.path.dirname(filename) != "":
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-    with open(filename, "w", encoding="utf-8") as file:
-        file.write("Total number of atoms\n")
-        file.write("%d\n" % len(structure))
-
-        # ^ write lattice info
-        if "LatticeFixs" in structure.sites[0].properties:
-            lfinfo = structure.sites[0].properties["LatticeFixs"]
-            if len(lfinfo) == 3:
-                file.write("Lattice Fix\n")
-                formatted_fts = []
-                for ft in lfinfo:
-                    if ft == "True":  # True
-                        ft_formatted = "T"
-                    else:
-                        ft_formatted = "F"
-                    formatted_fts.append(ft_formatted)
-                for v in structure.lattice.matrix:
-                    # write each element of formatted_fts in a line without [] symbol
-                    file.write(f'{v} {formatted_fts}.strip("[").strip("]")\n')
-            elif len(lfinfo) == 9:
-                file.write("Lattice Fix_x Fix_y Fix_z\n")
-                formatted_fts = []
-                for ft in lfinfo:
-                    if ft == "True":  # True
-                        ft_formatted = "T"
-                    else:
-                        ft_formatted = "F"
-                    formatted_fts.append(ft_formatted)
-                fix_str1 = " ".join(formatted_fts[:3])
-                fix_str2 = " ".join(formatted_fts[3:6])
-                fix_str3 = " ".join(formatted_fts[6:9])
-                v1 = structure.lattice.matrix[0]
-                v2 = structure.lattice.matrix[1]
-                v3 = structure.lattice.matrix[2]
-                file.write(f" {v1[0]:5.8f} {v1[1]:5.8f} {v1[2]:5.8f} {fix_str1}\n")
-                file.write(f" {v2[0]:5.8f} {v2[1]:5.8f} {v2[2]:5.8f} {fix_str2}\n")
-                file.write(f" {v3[0]:5.8f} {v3[1]:5.8f} {v3[2]:5.8f} {fix_str3}\n")
-            else:
-                raise ValueError(
-                    f"LatticeFixs should be a list of 3 or 9 bools, but got {lfinfo}"
-                )
-        else:
-            file.write("Lattice\n")
-            for v in structure.lattice.matrix:
-                file.write("%.8f %.8f %.8f\n" % (v[0], v[1], v[2]))
-
-        i = 0
-        for site in structure:
-            keys = []
-            for key in site.properties:  # site.properties is a dictionary
-                if key != "LatticeFixs":
-                    keys.append(key)
-            keys.sort()
-            keys_str = " ".join(keys)  # sth like 'magmom fix
-            if i == 0:
-                if coords_are_cartesian:
-                    file.write(f"Cartesian {keys_str}\n")
-                else:
-                    file.write(f"Direct {keys_str}\n")
-            i += 1
-
-            coords = site.coords if coords_are_cartesian else site.frac_coords
-            raw = []
-            for sortted_key in keys:  # site.properties is a dictionary
-                raw_values = site.properties[sortted_key]
-                # print(f'{raw_values=}')
-                if isinstance(raw_values, list):  # single True or False
-                    values = raw_values
-                else:
-                    values = [raw_values]
-                for v in values:
-                    if v == "True":
-                        value_str = "T"
-                    elif v == "False":
-                        value_str = "F"
-                    else:
-                        value_str = str(v)
-                    raw.append(value_str)
-
-            final_strs = " ".join(raw)  # sth like '0.0 T
-            file.write(
-                "%s %.8f %.8f %.8f %s\n"
-                % (site.species_string, coords[0], coords[1], coords[2], final_strs)
-            )
-
-
-def _to_hzw(structure, filename: str):
-    if os.path.isfile(filename):
-        print("Warning: %s already exists and will be overwritten!" % filename)
-    if os.path.dirname(filename) != "":
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-    with open(filename, "w", encoding="utf-8") as file:
-        file.write("% The number of probes \n")
-        file.write("0\n")
-        file.write("% Uni-cell vector\n")
-
-        for v in structure.lattice.matrix:
-            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
-
-        file.write("% Total number of device_structure\n")
-        file.write("%d\n" % len(structure))
-        file.write("% Atom site\n")
-
-        for site in structure:
-            file.write(
-                "%s %.6f %.6f %.6f\n"
-                % (site.species_string, site.coords[0], site.coords[1], site.coords[2])
-            )
-
-
-def _to_dspaw_json(structure, filename: str, coords_are_cartesian=True):
-    lattice = structure.lattice.matrix.flatten().tolist()
-    atoms = []
-    for site in structure:
-        coords = site.coords if coords_are_cartesian else site.frac_coords
-        atoms.append({"Element": site.species_string, "Position": coords.tolist()})
-
-    coordinate_type = "Cartesian" if coords_are_cartesian else "Direct"
-    d = {"Lattice": lattice, "CoordinateType": coordinate_type, "Atoms": atoms}
-    if os.path.isfile(filename):
-        print("Warning: %s already exists and will be overwritten!" % filename)
-    if os.path.dirname(filename) != "":
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-    with open(filename, "w", encoding="utf-8") as file:
-        json.dump(d, file, indent=4)
-
-
-def _to_pdb(structures, filename: str):
-    if not isinstance(structures, list):
-        structures = [structures]
-    if os.path.isfile(filename):
-        print("Warning: %s already exists and will be overwritten!" % filename)
-    if os.path.dirname(filename) != "":
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
-    with open(filename, "w", encoding="utf-8") as file:
-        for i, s in enumerate(structures):
-            file.write("MODEL         %d\n" % (i + 1))
-            file.write("REMARK   Converted from Structures\n")
-            file.write("REMARK   Converted using dspawpy\n")
-            lengths = s.lattice.lengths
-            angles = s.lattice.angles
-            file.write(
-                "CRYST1{0:9.3f}{1:9.3f}{2:9.3f}{3:7.2f}{4:7.2f}{5:7.2f}\n".format(
-                    lengths[0], lengths[1], lengths[2], angles[0], angles[1], angles[2]
-                )
-            )
-            for j, site in enumerate(s):
-                file.write(
-                    "%4s%7d%4s%5s%6d%4s%8.3f%8.3f%8.3f%6.2f%6.2f%12s\n"
-                    % (
-                        "ATOM",
-                        j + 1,
-                        site.species_string,
-                        "MOL",
-                        1,
-                        "    ",
-                        site.coords[0],
-                        site.coords[1],
-                        site.coords[2],
-                        1.0,
-                        0.0,
-                        site.species_string,
-                    )
-                )
-            file.write("TER\n")
-            file.write("ENDMDL\n")
+import json
+import os
+
+import numpy as np
+from pymatgen.core.structure import Structure
+
+from dspawpy.io.read import _get_lammps_non_orthogonal_box, load_h5
+
+
+def _write_xyz_traj(
+    structures,
+    xyzfile="aimdTraj.xyz",
+):
+    r"""保存xyz格式的轨迹文件
+
+    Parameters
+    ----------
+    structures: list
+        pymatgen的Structures列表
+    xyzfile : str
+        写入xyz格式的轨迹文件，默认为aimdTraj.xyz
+    """
+    if not isinstance(structures, list):  # single Structure
+        structures = [structures]
+    if os.path.isfile(xyzfile):
+        print("Warning: %s already exists and will be overwritten!" % xyzfile)
+    if os.path.dirname(xyzfile) != "":
+        os.makedirs(os.path.dirname(xyzfile), exist_ok=True)
+    with open(xyzfile, "w") as f:
+        # Nstep
+        for _, structure in enumerate(structures):
+            # 原子数不会变，就是不合并的元素总数
+            eles = [s.species_string for s in structure.sites]
+            f.write("%d\n" % len(eles))
+            # lattice
+            lm = structure.lattice.matrix
+            f.write(
+                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
+                % (
+                    lm[0, 0],
+                    lm[0, 1],
+                    lm[0, 2],
+                    lm[1, 0],
+                    lm[1, 1],
+                    lm[1, 2],
+                    lm[2, 0],
+                    lm[2, 1],
+                    lm[2, 2],
+                )
+            )
+            # position and element
+            poses = structure.cart_coords
+            for j in range(len(eles)):
+                f.write(
+                    "%s %f %f %f\n" % (eles[j], poses[j, 0], poses[j, 1], poses[j, 2])
+                )
+
+    print(f"{xyzfile} 文件已保存！")
+
+
+def _write_dump_traj(
+    structures,
+    dumpfile="aimdTraj.dump",
+):
+    r"""保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
+
+    Parameters
+    ----------
+    structures: list
+        pymatgen的Structures列表
+    dumpfile : str
+        dump格式的轨迹文件名，默认为aimdTraj.dump
+    """
+    if not isinstance(structures, list):  # single Structure
+        structures = [structures]
+    if os.path.isfile(dumpfile):
+        print("Warning: %s already exists and will be overwritten!" % dumpfile)
+    if os.path.dirname(dumpfile) != "":
+        os.makedirs(os.path.dirname(dumpfile), exist_ok=True)
+    with open(dumpfile, "w") as f:
+        for n, structure in enumerate(structures):
+            lat = structure.lattice.matrix
+            eles = [s.species_string for s in structure.sites]
+            poses = structure.cart_coords
+
+            box_bounds = _get_lammps_non_orthogonal_box(lat)
+            f.write("ITEM: TIMESTEP\n%d\n" % n)
+            f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
+            f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
+            f.write(
+                "%f %f %f\n%f %f %f\n %f %f %f\n"
+                % (
+                    box_bounds[0][0],
+                    box_bounds[0][1],
+                    box_bounds[0][2],
+                    box_bounds[1][0],
+                    box_bounds[1][1],
+                    box_bounds[1][2],
+                    box_bounds[2][0],
+                    box_bounds[2][1],
+                    box_bounds[2][2],
+                )
+            )
+            f.write("ITEM: ATOMS type x y z id\n")
+            for i in range(len(eles)):
+                f.write(
+                    "%s %f %f %f %d\n"
+                    % (
+                        eles[i],
+                        poses[i, 0],
+                        poses[i, 1],
+                        poses[i, 2],
+                        i + 1,
+                    )
+                )
+    print(f"{dumpfile} 文件已保存！")
+
+
+def write_VESTA(in_filename: str, data_type, out_filename="DS-PAW.vesta"):
+    """从包含电子体系信息的json或h5文件中读取数据并写入VESTA格式的文件中
+
+    Parameters
+    ----------
+    in_filename : str
+        包含电子体系信息的json或h5文件路径
+    data_type: str
+        数据类型，支持 "rho", "potential", "elf", "pcharge", "boundcharge"
+    out_filename : str
+        输出文件路径, 默认 "DS-PAW.vesta"
+
+    Returns
+    --------
+    out_filename : file
+        VESTA格式的文件
+
+    Examples
+    --------
+    >>> from dspawpy.io.write import write_VESTA
+    >>> write_VESTA("/data/home/hzw1002/dspawpy_repo/test/2.2/rho.json", "rho", out_filename='/data/home/hzw1002/dspawpy_repo/test/out/rho.json')
+    """
+    if in_filename.endswith(".h5"):
+        data = load_h5(in_filename)
+        if data_type.lower() == "rho" or data_type.lower() == "boundcharge":
+            _write_VESTA_format(data, ["/Rho/TotalCharge"], out_filename)
+        elif data_type.lower() == "potential":
+            _write_VESTA_format(
+                data,
+                [
+                    "/Potential/TotalElectrostaticPotential",
+                ],
+                out_filename,
+            )
+        elif data_type.lower() == "elf":
+            _write_VESTA_format(data, ["/ELF/TotalELF"], out_filename)
+        elif data_type.lower() == "pcharge":
+            _write_VESTA_format(data, ["/Pcharge/1/TotalCharge"], out_filename)
+        else:
+            raise NotImplementedError("仅支持rho/potential/elf/pcharge/boundcharge")
+
+    elif in_filename.endswith(".json"):
+        with open(in_filename, "r") as fin:
+            data = json.load(fin)
+        if data_type.lower() == "rho" or data_type.lower() == "boundcharge":
+            _write_VESTA_format_json(
+                data["AtomInfo"], [data["Rho"]["TotalCharge"]], out_filename
+            )
+        elif data_type.lower() == "potential":
+            _write_VESTA_format_json(
+                data["AtomInfo"],
+                [
+                    data["Potential"]["TotalElectrostaticPotential"],
+                ],
+                out_filename,
+            )
+        elif data_type.lower() == "elf":
+            _write_VESTA_format_json(
+                data["AtomInfo"], [data["ELF"]["TotalELF"]], out_filename
+            )
+        elif data_type.lower() == "pcharge":
+            _write_VESTA_format_json(
+                data["AtomInfo"], [data["Pcharge"][0]["TotalCharge"]], out_filename
+            )
+        else:
+            raise NotImplementedError("仅支持rho/potential/elf/pcharge/boundcharge")
+
+    else:
+        raise NotImplementedError("仅支持json或h5格式文件")
+
+
+def write_delta_rho_vesta(AB, A, B, output="delta_rho.vesta"):
+    """电荷密度差分可视化
+
+    DeviceStudio暂不支持大文件，临时写成可以用VESTA打开的格式
+
+    Parameters
+    ----------
+    AB : str
+        AB的电荷密度文件路径，可以是h5或json格式
+    A : str
+        A的电荷密度文件路径，可以是h5或json格式
+    B : str
+        B的电荷密度文件路径，可以是h5或json格式
+    output : str
+        输出文件路径，默认 "delta_rho.vesta"
+
+    Returns
+    -------
+    output : file
+        电荷差分（AB-A-B）后的电荷密度文件，
+
+    Examples
+    --------
+    >>> from dspawpy.io.write import write_delta_rho_vesta
+    >>> write_delta_rho_vesta('/data/home/hzw1002/dspawpy_repo/test/supplement/AB.h5', '/data/home/hzw1002/dspawpy_repo/test/supplement/A.h5', '/data/home/hzw1002/dspawpy_repo/test/supplement/B.h5', '/data/home/hzw1002/dspawpy_repo/test/out/delta_rho.vesta')
+    读取/data/home/hzw1002/dspawpy_repo/test/supplement/AB.h5...
+    读取/data/home/hzw1002/dspawpy_repo/test/supplement/A.h5...
+    读取/data/home/hzw1002/dspawpy_repo/test/supplement/B.h5...
+    计算电荷差分...
+    写入文件/data/home/hzw1002/dspawpy_repo/test/out/delta_rho.vesta...
+    成功写入 /data/home/hzw1002/dspawpy_repo/test/out/delta_rho.vesta
+    """
+    print(f"读取{AB}...")
+    if AB.endswith(".h5"):
+        dataAB = load_h5(AB)
+        rhoAB = np.array(dataAB["/Rho/TotalCharge"])
+        nGrids = dataAB["/AtomInfo/Grid"]
+        atom_symbol = dataAB["/AtomInfo/Elements"]
+        atom_pos = dataAB["/AtomInfo/Position"]
+        latticeConstantMatrix = dataAB["/AtomInfo/Lattice"]
+        atom_pos = np.array(atom_pos).reshape(-1, 3)
+    elif AB.endswith(".json"):
+        atom_symbol = []
+        atom_pos = []
+        with open(AB, "r") as f1:
+            dataAB = json.load(f1)
+            rhoAB = np.array(dataAB["Rho"]["TotalCharge"])
+            nGrids = dataAB["AtomInfo"]["Grid"]
+        for i in range(len(dataAB["AtomInfo"]["Atoms"])):
+            atom_symbol.append(dataAB["AtomInfo"]["Atoms"][i]["Element"])
+            atom_pos.append(dataAB["AtomInfo"]["Atoms"][i]["Position"])
+        atom_pos = np.array(atom_pos)
+
+        latticeConstantMatrix = dataAB["AtomInfo"]["Lattice"]
+    else:
+        raise ValueError(f"file format must be either h5 or json: {AB}")
+
+    print(f"读取{A}...")
+    if A.endswith(".h5"):
+        dataA = load_h5(A)
+        rhoA = np.array(dataA["/Rho/TotalCharge"])
+    elif A.endswith(".json"):
+        with open(A, "r") as f2:
+            dataA = json.load(f2)
+            rhoA = np.array(dataA["Rho"]["TotalCharge"])
+    else:
+        raise ValueError(f"file format must be either h5 or json: {A}")
+
+    print(f"读取{B}...")
+    if B.endswith(".h5"):
+        dataB = load_h5(B)
+        rhoB = np.array(dataB["/Rho/TotalCharge"])
+    elif B.endswith(".json"):
+        with open(B, "r") as f3:
+            dataB = json.load(f3)
+            rhoB = np.array(dataB["Rho"]["TotalCharge"])
+    else:
+        raise ValueError(f"file format must be either h5 or json: {B}")
+
+    print(f"计算电荷差分...")
+    rho = rhoAB - rhoA - rhoB
+    rho = np.array(rho).reshape(nGrids[0], nGrids[1], nGrids[2])
+    element = list(set(atom_symbol))
+    element = sorted(set(atom_symbol), key=atom_symbol.index)
+    element_num = np.zeros(len(element))
+    for i in range(len(element)):
+        element_num[i] = atom_symbol.count(element[i])
+
+    latticeConstantMatrix = np.array(latticeConstantMatrix)
+    latticeConstantMatrix = latticeConstantMatrix.reshape(3, 3)
+
+    print(f"写入文件{output}...")
+    if os.path.isfile(output):
+        print("Warning: %s already exists and will be overwritten!" % output)
+    if os.path.dirname(output) != "":
+        os.makedirs(os.path.dirname(output), exist_ok=True)
+    with open(output, "w") as out:
+        out.write("DS-PAW_rho\n")
+        out.write("    1.000000\n")
+        for i in range(3):
+            for j in range(3):
+                out.write("    " + str(latticeConstantMatrix[i, j]) + "    ")
+            out.write("\n")
+        for i in range(len(element)):
+            out.write("    " + element[i] + "    ")
+        out.write("\n")
+
+        for i in range(len(element_num)):
+            out.write("    " + str(int(element_num[i])) + "    ")
+        out.write("\n")
+        out.write("Direct\n")
+        for i in range(len(atom_pos)):
+            for j in range(3):
+                out.write("    " + str(atom_pos[i, j]) + "    ")
+            out.write("\n")
+        out.write("\n")
+
+        for i in range(3):
+            out.write("  " + str(nGrids[i]) + "  ")
+        out.write("\n")
+
+        ind = 0
+        for i in range(nGrids[0]):
+            for j in range(nGrids[1]):
+                for k in range(nGrids[2]):
+                    out.write("  " + str(rho[i, j, k]) + "  ")
+                    ind = ind + 1
+                    if ind % 5 == 0:
+                        out.write("\n")
+
+    print(f"成功写入 {output}")
+
+
+def to_file(structure, filename: str, fmt=None, coords_are_cartesian=True, si=None):
+    r"""往结构文件中写入信息
+
+    Parameters
+    ----------
+    structure : Structure
+        pymatgen的Structure对象
+    filename : str
+        结构文件名
+    fmt : str
+        - 结构文件类型，原生支持 'json', 'as', 'hzw', 'pdb', 'xyz', 'dump' 六种
+    coords_are_cartesian : bool
+        - 是否写作笛卡尔坐标，默认为True；否则写成分数坐标形式
+        - 此选项暂时仅对 as 和 json 格式有效
+    si : int
+        结构编号索引
+
+    Examples
+    --------
+
+    先读取结构信息:
+
+    >>> from dspawpy.io.structure import build_Structures_from_datafile
+    >>> s = build_Structures_from_datafile('/data/home/hzw1002/dspawpy_repo/test/2.15/01/neb01.h5')
+    Reading /data/home/hzw1002/dspawpy_repo/test/2.15/01/neb01.h5...
+    >>> len(s)
+    17
+
+    将结构信息写入文件：
+
+    >>> from dspawpy.io.write import to_file
+    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.json', coords_are_cartesian=True)
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.json
+    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.as', coords_are_cartesian=True)
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.as
+    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.hzw', coords_are_cartesian=True)
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.hzw
+
+    pdb, xyz, dump 三种类型的文件，可以写入多个构型，形成“轨迹”。生成的 xyz 等轨迹文件可使用 OVITO 等可视化软件打开观察。
+
+    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.pdb', coords_are_cartesian=True)
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.pdb
+    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.xyz', coords_are_cartesian=True)
+    /data/home/hzw1002/dspawpy_repo/test/out/PtH.xyz 文件已保存！
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.xyz
+    >>> to_file(s, filename='/data/home/hzw1002/dspawpy_repo/test/out/PtH.dump', coords_are_cartesian=True)
+    /data/home/hzw1002/dspawpy_repo/test/out/PtH.dump 文件已保存！
+    --> 成功写入文件 /data/home/hzw1002/dspawpy_repo/test/out/PtH.dump
+
+    单结构信息推荐使用 as 格式存储，如果 Structure 中有磁矩或自由度信息，将会按最完整的格式统一写入，形如 Fix_x, Fix_y, Fix_z, Mag_x, Mag_y, Mag_z，自由度信息默认为 F，磁矩默认为 0.0。可视情况自行手动删除生成的 as 文件中的这些默认信息
+
+    >>> with open('/data/home/hzw1002/dspawpy_repo/test/out/PtH.as') as f:
+    ...     print(f.read())
+    ...
+    Total number of atoms
+    13
+    Lattice Fix_x Fix_y Fix_z
+     5.60580000 0.00000000 0.00000000 F F F
+     0.00000000 5.60580000 0.00000000 F F F
+     0.00000000 0.00000000 16.81740000 F F F
+    Cartesian Fix_x Fix_y Fix_z Mag
+    H 2.58985263 3.72755271 6.94246998 F F F 0.0
+    Pt 1.37942121 1.39655502 1.96304099 F F F 0.0
+    Pt 4.20055071 1.40326436 1.94681875 F F F 0.0
+    Pt 1.37462277 4.20932677 2.00221003 F F F 0.0
+    Pt 4.21197615 4.21324064 1.99578112 F F F 0.0
+    Pt 5.58740047 5.59517338 3.93274445 F F F 0.0
+    Pt 5.58633749 2.78068345 3.91301343 F F F 0.0
+    Pt 2.79076605 5.59305895 3.91208092 F F F 0.0
+    Pt 2.78904685 2.78501463 3.89610696 F F F 0.0
+    Pt 1.38102265 1.36691874 5.84326681 F F F 0.0
+    Pt 4.19057728 1.36788897 5.84877666 F F F 0.0
+    Pt 1.34667410 4.16198043 5.89298591 F F F 0.0
+    Pt 4.17046728 4.15729941 5.89874209 F F F 0.0
+    <BLANKLINE>
+
+    写成其他类型的结构文件，将忽略磁矩和自由度信息
+    """
+    if si is not None:
+        assert isinstance(si, int), "si 应当是用于索引列表的整数"
+    if isinstance(structure, Structure):
+        structure = [structure]
+
+    if fmt is None:
+        fmt = filename.split(".")[-1]
+
+    if fmt == "pdb":  # 可以是多个构型
+        if si:
+            _to_pdb(structure[si], filename)
+        else:
+            _to_pdb(structure, filename)
+    elif fmt == "xyz":  # 可以是多个构型
+        if si:
+            _write_xyz_traj(structure[si], filename)
+        else:
+            _write_xyz_traj(structure, filename)
+    elif fmt == "dump":  # 可以是多个构型
+        if si:
+            _write_dump_traj(structure[si], filename)
+        else:
+            _write_dump_traj(structure, filename)
+
+    elif fmt == "json":  # 单个构型
+        if si:
+            _to_dspaw_json(structure[si], filename, coords_are_cartesian)
+        else:
+            _to_dspaw_json(structure[-1], filename, coords_are_cartesian)
+    elif fmt == "as":
+        if si:
+            _to_dspaw_as(structure[si], filename, coords_are_cartesian)
+        else:
+            _to_dspaw_as(structure[-1], filename, coords_are_cartesian)
+    elif fmt == "hzw":
+        if si:
+            _to_hzw(structure[si], filename)
+        else:
+            _to_hzw(structure[-1], filename)
+
+    elif fmt in [
+        "cif",
+        "mcif",
+        "poscar",
+        "cssr",
+        "xsf",
+        "mcsqs",
+        "yaml",
+        "fleur-inpgen",
+        "prismatic",
+        "res",
+    ]:
+        if si:
+            structure[si].to(filename, fmt=fmt)
+        else:
+            structure[-1].to(filename, fmt=fmt)
+
+    else:
+        try:
+            if si:
+                structure[si].to(filename)
+            else:
+                structure[-1].to(filename)
+        except Exception as e:
+            raise NotImplementedError(
+                f"除了 pdb, xyz, dump, json, as, hzw 六种格式外，其他格式一律移交 pymatgen 处理，然而\n--> pymatgen返回错误：{e}"
+            )
+
+    print(f"--> 成功写入文件 {os.path.abspath(filename)}")
+
+
+def _write_atoms(fileobj, hdf5):
+    fileobj.write("DS-PAW Structure\n")
+    fileobj.write("  1.00\n")
+    lattice = np.asarray(hdf5["/AtomInfo/Lattice"]).reshape(-1, 1)  # 将列表lattice下的多个列表整合
+    fileobj.write(
+        "%10.6f %10.6f %10.6f\n" % (lattice[0][0], lattice[1][0], lattice[2][0])
+    )
+    fileobj.write(
+        "%10.6f %10.6f %10.6f\n" % (lattice[3][0], lattice[4][0], lattice[5][0])
+    )
+    fileobj.write(
+        "%10.6f %10.6f %10.6f\n" % (lattice[6][0], lattice[7][0], lattice[8][0])
+    )
+
+    elements = hdf5["/AtomInfo/Elements"]
+    elements_set = []
+    elements_number = {}
+    for e in elements:
+        if e in elements_set:
+            elements_number[e] = elements_number[e] + 1
+        else:
+            elements_set.append(e)
+            elements_number[e] = 1
+
+    for e in elements_set:
+        fileobj.write("  " + e)
+    fileobj.write("\n")
+
+    for e in elements_set:
+        fileobj.write("%5d" % (elements_number[e]))
+    fileobj.write("\n")
+    if hdf5["/AtomInfo/CoordinateType"][0] == "Direct":
+        fileobj.write("Direct\n")
+    else:
+        fileobj.write("Cartesian\n")
+    for i, p in enumerate(hdf5["/AtomInfo/Position"]):
+        fileobj.write("%10.6f" % p)
+        if (i + 1) % 3 == 0:
+            fileobj.write("\n")
+    fileobj.write("\n")
+
+
+def _write_VESTA_format(hdf5: dict, datakeys: list, filename):
+    if os.path.isfile(filename):
+        print("Warning: %s already exists and will be overwritten!" % filename)
+    if os.path.dirname(filename) != "":
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    with open(filename, "w") as file:
+        _write_atoms(file, hdf5)
+        for key in datakeys:
+            d = np.asarray(hdf5[key]).reshape(-1, 1)  # 将列表hdf5[key]下的多个列表整合
+            file.write("%5d %5d %5d\n" % tuple(hdf5["/AtomInfo/Grid"]))
+            i = 0
+            while i < len(d):
+                for j in range(10):
+                    file.write("%10.5f " % d[i])
+                    i += 1
+                    if i >= len(d):
+                        break
+                file.write("\n")
+
+            file.write("\n")
+
+
+def _write_atoms_json(fileobj, atom_info):
+    fileobj.write("DS-PAW Structure\n")
+    fileobj.write("  1.00\n")
+    lattice = atom_info["Lattice"]
+
+    fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[0], lattice[1], lattice[2]))
+    fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[3], lattice[4], lattice[5]))
+    fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[6], lattice[7], lattice[8]))
+
+    elements = [atom["Element"] for atom in atom_info["Atoms"]]
+    elements_set = []
+    elements_number = {}
+    for e in elements:
+        if e in elements_set:
+            elements_number[e] = elements_number[e] + 1
+        else:
+            elements_set.append(e)
+            elements_number[e] = 1
+
+    for e in elements_set:
+        fileobj.write("  " + e)
+    fileobj.write("\n")
+
+    for e in elements_set:
+        fileobj.write("%5d" % (elements_number[e]))
+    fileobj.write("\n")
+    if atom_info["CoordinateType"] == "Direct":
+        fileobj.write("Direct\n")
+    else:
+        fileobj.write("Cartesian\n")
+    for atom in atom_info["Atoms"]:
+        fileobj.write("%10.6f %10.6f %10.6f\n" % tuple(atom["Position"]))
+    fileobj.write("\n")
+
+
+def _write_VESTA_format_json(atom_info: dict, data: list, filename):
+    if os.path.isfile(filename):
+        print("Warning: %s already exists and will be overwritten!" % filename)
+    if os.path.dirname(filename) != "":
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    with open(filename, "w") as file:
+        _write_atoms_json(file, atom_info)
+        for d in data:
+            file.write("%5d %5d %5d\n" % tuple(atom_info["Grid"]))
+            i = 0
+            while i < len(d):
+                for j in range(10):
+                    file.write("%10.5f " % d[i])
+                    i += 1
+                    if i >= len(d):
+                        break
+                file.write("\n")
+
+            file.write("\n")
+
+
+def _to_dspaw_as(structure, filename: str, coords_are_cartesian=True):
+    """write dspaw structure file of .as type"""
+    if os.path.isfile(filename):
+        print("Warning: %s already exists and will be overwritten!" % filename)
+    if os.path.dirname(filename) != "":
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    with open(filename, "w", encoding="utf-8") as file:
+        file.write("Total number of atoms\n")
+        file.write("%d\n" % len(structure))
+
+        # ^ write lattice info
+        if "LatticeFixs" in structure.sites[0].properties:
+            lfinfo = structure.sites[0].properties["LatticeFixs"]
+            if len(lfinfo) == 3:
+                file.write("Lattice Fix\n")
+                formatted_fts = []
+                for ft in lfinfo:
+                    if ft == "True":  # True
+                        ft_formatted = "T"
+                    else:
+                        ft_formatted = "F"
+                    formatted_fts.append(ft_formatted)
+                for v in structure.lattice.matrix:
+                    # write each element of formatted_fts in a line without [] symbol
+                    file.write(f'{v} {formatted_fts}.strip("[").strip("]")\n')
+            elif len(lfinfo) == 9:
+                file.write("Lattice Fix_x Fix_y Fix_z\n")
+                formatted_fts = []
+                for ft in lfinfo:
+                    if ft == "True":  # True
+                        ft_formatted = "T"
+                    else:
+                        ft_formatted = "F"
+                    formatted_fts.append(ft_formatted)
+                fix_str1 = " ".join(formatted_fts[:3])
+                fix_str2 = " ".join(formatted_fts[3:6])
+                fix_str3 = " ".join(formatted_fts[6:9])
+                v1 = structure.lattice.matrix[0]
+                v2 = structure.lattice.matrix[1]
+                v3 = structure.lattice.matrix[2]
+                file.write(f" {v1[0]:5.8f} {v1[1]:5.8f} {v1[2]:5.8f} {fix_str1}\n")
+                file.write(f" {v2[0]:5.8f} {v2[1]:5.8f} {v2[2]:5.8f} {fix_str2}\n")
+                file.write(f" {v3[0]:5.8f} {v3[1]:5.8f} {v3[2]:5.8f} {fix_str3}\n")
+            else:
+                raise ValueError(
+                    f"LatticeFixs should be a list of 3 or 9 bools, but got {lfinfo}"
+                )
+        else:
+            file.write("Lattice\n")
+            for v in structure.lattice.matrix:
+                file.write("%.8f %.8f %.8f\n" % (v[0], v[1], v[2]))
+
+        i = 0
+        for site in structure:
+            keys = []
+            for key in site.properties:  # site.properties is a dictionary
+                if key != "LatticeFixs":
+                    keys.append(key)
+            keys.sort()
+            keys_str = " ".join(keys)  # sth like 'magmom fix
+            if i == 0:
+                if coords_are_cartesian:
+                    file.write(f"Cartesian {keys_str}\n")
+                else:
+                    file.write(f"Direct {keys_str}\n")
+            i += 1
+
+            coords = site.coords if coords_are_cartesian else site.frac_coords
+            raw = []
+            for sortted_key in keys:  # site.properties is a dictionary
+                raw_values = site.properties[sortted_key]
+                # print(f'{raw_values=}')
+                if isinstance(raw_values, list):  # single True or False
+                    values = raw_values
+                else:
+                    values = [raw_values]
+                for v in values:
+                    if v == "True":
+                        value_str = "T"
+                    elif v == "False":
+                        value_str = "F"
+                    else:
+                        value_str = str(v)
+                    raw.append(value_str)
+
+            final_strs = " ".join(raw)  # sth like '0.0 T
+            file.write(
+                "%s %.8f %.8f %.8f %s\n"
+                % (site.species_string, coords[0], coords[1], coords[2], final_strs)
+            )
+
+
+def _to_hzw(structure, filename: str):
+    if os.path.isfile(filename):
+        print("Warning: %s already exists and will be overwritten!" % filename)
+    if os.path.dirname(filename) != "":
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    with open(filename, "w", encoding="utf-8") as file:
+        file.write("% The number of probes \n")
+        file.write("0\n")
+        file.write("% Uni-cell vector\n")
+
+        for v in structure.lattice.matrix:
+            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
+
+        file.write("% Total number of device_structure\n")
+        file.write("%d\n" % len(structure))
+        file.write("% Atom site\n")
+
+        for site in structure:
+            file.write(
+                "%s %.6f %.6f %.6f\n"
+                % (site.species_string, site.coords[0], site.coords[1], site.coords[2])
+            )
+
+
+def _to_dspaw_json(structure, filename: str, coords_are_cartesian=True):
+    lattice = structure.lattice.matrix.flatten().tolist()
+    atoms = []
+    for site in structure:
+        coords = site.coords if coords_are_cartesian else site.frac_coords
+        atoms.append({"Element": site.species_string, "Position": coords.tolist()})
+
+    coordinate_type = "Cartesian" if coords_are_cartesian else "Direct"
+    d = {"Lattice": lattice, "CoordinateType": coordinate_type, "Atoms": atoms}
+    if os.path.isfile(filename):
+        print("Warning: %s already exists and will be overwritten!" % filename)
+    if os.path.dirname(filename) != "":
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    with open(filename, "w", encoding="utf-8") as file:
+        json.dump(d, file, indent=4)
+
+
+def _to_pdb(structures, filename: str):
+    if not isinstance(structures, list):
+        structures = [structures]
+    if os.path.isfile(filename):
+        print("Warning: %s already exists and will be overwritten!" % filename)
+    if os.path.dirname(filename) != "":
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    with open(filename, "w", encoding="utf-8") as file:
+        for i, s in enumerate(structures):
+            file.write("MODEL         %d\n" % (i + 1))
+            file.write("REMARK   Converted from Structures\n")
+            file.write("REMARK   Converted using dspawpy\n")
+            lengths = s.lattice.lengths
+            angles = s.lattice.angles
+            file.write(
+                "CRYST1{0:9.3f}{1:9.3f}{2:9.3f}{3:7.2f}{4:7.2f}{5:7.2f}\n".format(
+                    lengths[0], lengths[1], lengths[2], angles[0], angles[1], angles[2]
+                )
+            )
+            for j, site in enumerate(s):
+                file.write(
+                    "%4s%7d%4s%5s%6d%4s%8.3f%8.3f%8.3f%6.2f%6.2f%12s\n"
+                    % (
+                        "ATOM",
+                        j + 1,
+                        site.species_string,
+                        "MOL",
+                        1,
+                        "    ",
+                        site.coords[0],
+                        site.coords[1],
+                        site.coords[2],
+                        1.0,
+                        0.0,
+                        site.species_string,
+                    )
+                )
+            file.write("TER\n")
+            file.write("ENDMDL\n")
```

## Comparing `dspawpy-0.9.8.dist-info/METADATA` & `dspawpy-0.9.9.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-Metadata-Version: 2.1
-Name: dspawpy
-Version: 0.9.8
-Summary: Tools for dspaw
-Home-page: http://www.hzwtech.com/
-Author: Hzwtech
-License: MIT
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-Requires-Dist: pymatgen (>=2021.2.8.1)
-Requires-Dist: statsmodels (>=0.12.0)
-Requires-Dist: h5py (>=3.7)
-Requires-Dist: joblib
-
-# 简介
-
-dspawpy 是 DS-PAW 的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能
-
-## 安装提示
-
-如果普通pip可以安装dspawpy，但是conda环境中的pip无法安装，报错
-
-ERROR: Could not find a version that satisfies the requirement dspawpy
-
-那么，尝试升级conda和pip
-
-```sh
-
-conda update conda
-conda update pip
-```
-
-再重新用pip安装。
-
-详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
-
-## 版本更新简述
-
-### 0.9.8
-
-- BUG修复： to_file 和 build_Structures_from_datafile 接口统一
-- BUG修复： io.write模块涉及的保存文件操作，当目标路径上层文件夹不存在时将自动创建
-- BUG修复： io.read.get_band_data的zero_to_efermi参数设置为True时，数据的处理逻辑
-- BUG修复： io.read.get_sinfo读取relax.json不再因FixLattice而报错
-- 新增选项： nebtools的summary函数，新增show_converge用于控制是否显示收敛图，outdir用于指定收敛图的路径
-- 新增功能： 写文件涉及的操作，支持传入路径，而不单是文件名
-- 新增功能： nebtools的restart函数支持在Windows机器上操作，不必在旧NEB路径执行，备份路径可随意指定
-- 新增功能： nebtools的get_neb_subfolder函数新增return_abs参数，用于返回子文件夹的绝对路径
-- 重要变更： nebtools的restart函数删除inputin参数，采用压缩较快的zip方法，将生成zip压缩包而不是tar.xz
-- 重要变更： io.read.get_band_data的zero_to_fermi参数改名zero_to_efermi
-
-### 0.9.7
-
-- BUG修复： get_rdf 元素对自己计算RDF时的索引
-- 新增选项：to_file 增加 si 参数，支持读入单个structure以及Structure列表
-
-### 0.9.6
-
-- BUG修复： pymatgen支持的几类结构文件的读取接口
-
-### 0.9.5
-
-- 重要变更： get_band_data 的 shift_efermi 参数改名为 zero_to_fermi
-
-### 0.9.4
-
-- 新增功能： get_band_data 增加 shift_efermi 参数
-- BUG修复： 电荷密度差分函数移除 numpy 多维数组的 shape 参数
-- BUG修复： Fe_1 -> Fe+, Fe_2 -> Fe2+ 用于能带、态密度绘图
-
-### 0.9.3
-
-- 新增功能： 接入pymatgen支持的几类结构文件的读写操作
-- 新增功能： 支持通过 `dspawpy.__version__` 查看版本号
-- 重要变更： write_xyz_traj, write_dump_traj 并入 to_file 函数
-- 细节优化： 大幅提高RDF计算效率
-
-### 0.9.2
-
-- 新增功能： 支持从as文件中解析磁矩和FIX信息
-- 新增功能： 从h5/json文件中读取数据时支持指定读取的离子步（从1开始）
-
-### 0.9.1
-
-- 重要变更： 精简合并多个函数，统一调用方法
-- 新增功能： 支持合并多个xyz和dump文件
-- 细节优化： 读取h5或json文件后若无错误，不再打印空行
-- 细节优化： 耗时的RDF计算显示进度百分比
-
-### 0.9.0
-
-- 重要变更： 一些函数合并、所在模块迁移，请确认版本
-- 新增功能： 支持读取含多离子步计算结果的h5/json文件中的磁矩信息
-- BUG修复： get_band_data 函数指定efermi不生效
-
-### 0.8.9
-
-- BUG修复： d_band 脚本运行错误
-
-### 0.8.8
-
-- 新增功能： 支持读取正在进行中的NEB信息，生成movie轨迹文件（可用DS打开观察）
-- 新增功能： 支持NEB转XYZ轨迹文件（可用OVITO打开观察）
-- 新增功能： plot_aimd 支持读取多个h5文件画在同一张图中
-- BUG修复： 电荷差分处理json文件报错
-- BUG修复： 极化曲线标记的数值错误
-- BUG修复： neb_movie_*.json 中反应坐标重复累加错误
-
-### 0.8.7
-
-- 代码重构，大幅修改数据结构，加速处理过程
-- 支持读取h5格式的输出文件
-- 新增AIMD, NEB等部分常用功能
-
-### 0.3.0
-
-- 对应2021A版本DS-PAW，辅助处理一些常见数据文件
+Metadata-Version: 2.1
+Name: dspawpy
+Version: 0.9.9
+Summary: Tools for dspaw
+Home-page: http://www.hzwtech.com/
+Author: Hzwtech
+License: MIT
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+Requires-Dist: pymatgen (>=2021.2.8.1)
+Requires-Dist: statsmodels (>=0.12.0)
+Requires-Dist: h5py (>=3.7)
+
+# 简介
+
+dspawpy 是 DS-PAW 的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能
+
+## 安装提示
+
+如果普通pip可以安装dspawpy，但是conda环境中的pip无法安装，报错
+
+ERROR: Could not find a version that satisfies the requirement dspawpy
+
+那么，尝试升级conda和pip
+
+```sh
+
+conda update conda
+conda update pip
+```
+
+再重新用pip安装。
+
+详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
+
+## 版本更新简述
+
+### 0.9.9
+
+- BUG修复： 修复新版numpy不支持混用array和list生成数组的问题
+- 新增功能： build_Structures_from_datafile模块支持读取 neb.h5 和 phonon.h5 文件
+- 重要变更： 移除io模块中冗余的 _json.py （相关功能已整合进其他模块中并有所加强）
+- 重要变更： 删除 setup.py 中不需要的 joblib 依赖库
+
+### 0.9.8
+
+- BUG修复： to_file 和 build_Structures_from_datafile 接口统一
+- BUG修复： io.write模块涉及的保存文件操作，当目标路径上层文件夹不存在时将自动创建
+- BUG修复： io.read.get_band_data的zero_to_efermi参数设置为True时，数据的处理逻辑
+- BUG修复： io.read.get_sinfo读取relax.json不再因FixLattice而报错
+- 新增选项： nebtools的summary函数，新增show_converge用于控制是否显示收敛图，outdir用于指定收敛图的路径
+- 新增功能： 写文件涉及的操作，支持传入路径，而不单是文件名
+- 新增功能： nebtools的restart函数支持在Windows机器上操作，不必在旧NEB路径执行，备份路径可随意指定
+- 新增功能： nebtools的get_neb_subfolder函数新增return_abs参数，用于返回子文件夹的绝对路径
+- 重要变更： nebtools的restart函数删除inputin参数，采用压缩较快的zip方法，将生成zip压缩包而不是tar.xz
+- 重要变更： io.read.get_band_data的zero_to_fermi参数改名zero_to_efermi
+
+### 0.9.7
+
+- BUG修复： get_rdf 元素对自己计算RDF时的索引
+- 新增选项：to_file 增加 si 参数，支持读入单个structure以及Structure列表
+
+### 0.9.6
+
+- BUG修复： pymatgen支持的几类结构文件的读取接口
+
+### 0.9.5
+
+- 重要变更： get_band_data 的 shift_efermi 参数改名为 zero_to_fermi
+
+### 0.9.4
+
+- 新增功能： get_band_data 增加 shift_efermi 参数
+- BUG修复： 电荷密度差分函数移除 numpy 多维数组的 shape 参数
+- BUG修复： Fe_1 -> Fe+, Fe_2 -> Fe2+ 用于能带、态密度绘图
+
+### 0.9.3
+
+- 新增功能： 接入pymatgen支持的几类结构文件的读写操作
+- 新增功能： 支持通过 `dspawpy.__version__` 查看版本号
+- 重要变更： write_xyz_traj, write_dump_traj 并入 to_file 函数
+- 细节优化： 大幅提高RDF计算效率
+
+### 0.9.2
+
+- 新增功能： 支持从as文件中解析磁矩和FIX信息
+- 新增功能： 从h5/json文件中读取数据时支持指定读取的离子步（从1开始）
+
+### 0.9.1
+
+- 重要变更： 精简合并多个函数，统一调用方法
+- 新增功能： 支持合并多个xyz和dump文件
+- 细节优化： 读取h5或json文件后若无错误，不再打印空行
+- 细节优化： 耗时的RDF计算显示进度百分比
+
+### 0.9.0
+
+- 重要变更： 一些函数合并、所在模块迁移，请确认版本
+- 新增功能： 支持读取含多离子步计算结果的h5/json文件中的磁矩信息
+- BUG修复： get_band_data 函数指定efermi不生效
+
+### 0.8.9
+
+- BUG修复： d_band 脚本运行错误
+
+### 0.8.8
+
+- 新增功能： 支持读取正在进行中的NEB信息，生成movie轨迹文件（可用DS打开观察）
+- 新增功能： 支持NEB转XYZ轨迹文件（可用OVITO打开观察）
+- 新增功能： plot_aimd 支持读取多个h5文件画在同一张图中
+- BUG修复： 电荷差分处理json文件报错
+- BUG修复： 极化曲线标记的数值错误
+- BUG修复： neb_movie_*.json 中反应坐标重复累加错误
+
+### 0.8.7
+
+- 代码重构，大幅修改数据结构，加速处理过程
+- 支持读取h5格式的输出文件
+- 新增AIMD, NEB等部分常用功能
+
+### 0.3.0
+
+- 对应2021A版本DS-PAW，辅助处理一些常见数据文件
```

