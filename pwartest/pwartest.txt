# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Wooldridge Test for AR(1) Errors in FE Panel Models Use pwartest (plm) With (In) R Software
install.packages("plm")
library("plm")
# Estimation Wooldridge Test for AR(1) Errors in FE Panel Models Use pwartest (plm) With (In) R Software
pwartest = read.csv("https://raw.githubusercontent.com/timbulwidodostp/pwartest/main/pwartest/pwartest.csv",sep = ";")
Fixed = plm (Dependen ~ Indenpenden_1 + Indenpenden_2, data = pwartest, effect = "twoways",model = "within")
pwartest <- pwartest(Fixed)
pwartest
pwartest_ <- pwartest(Fixed, type = "HC3")
pwartest_
# Wooldridge Test for AR(1) Errors in FE Panel Models Use pwartest (plm) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished