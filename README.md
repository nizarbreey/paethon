# paethon
import matplotlib.pyplot as plt
import numpy as np

# إنشاء قلب باستخدام دوائر
theta = np.linspace(0, 4*np.pi, 200)
a = 0.5
r = 1 - a * np.abs(np.cos(theta))

x = r * np.cos( theta )
y = r * np.sin( theta )

# رسم القلب
plt.plot(x, y, color='pink')

# كتابة النص داخل القلب
plt.text(0, -0.5, "أحبك لولي", fontsize=20, fontweight='bold', color='white', ha='center', va='center')

# إظهار الرسم
plt.axis('off')
plt.show()

